<template>
    <div id="form">
        <form>
            <input  type="search"
                    placeholder="Search Your Movie"
                    class="form-control"
                    ref="movieName"
            />
            <input  type="submit"
                    value="Search"
                    class="btn"
                    @click.prevent="fetchMovie"
            />
        </form>
        <Movies :movies="allMovies" />
    </div>
</template>

<script>
import Movies from "@/components/App-Movies.vue";
import axios from 'axios';
export default {
    data() {
        return {
            allMovies: []
        }
    },
    methods: {
        fetchMovie: function() {
            var movieName = this.$refs.movieName.value;
            axios.get(`https://www.omdbapi.com/?s=${movieName}&apikey=981eb563`).then(response => {
                this.allMovies = response.data.Search;
                console.log(response.data.Search);
            })
        }
    },
    components: {
        Movies
    }
}
</script>

<style scoped lang="scss">
#form {
    margin-top: 20px;
    padding-bottom: 10px;
    form {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        input {
            &[type="search"] {
                width: 80%;
                outline: none;
                box-shadow: none;
                border: 1px solid #42b983;
            }
            &[type="submit"] {
                background-color: #42b983;
                color: white;
                width: 300px;
                margin-top: 10px;
            }
        }
    }
}
</style>