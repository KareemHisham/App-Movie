<template>
    <div id="form">
        <form>
            <input type="search" placeholder="Search Your Movie" class="form-control" />
            <input type="submit" value="Search" class="btn" />
        </form>
    </div>
</template>

<script>
export default {
    
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