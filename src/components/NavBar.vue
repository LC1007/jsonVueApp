<template>
    <div>
        <nav>
            <ul>
                <a href="#"><li>Home</li></a>
                <a href="#"><li>About</li></a>
            </ul>
        </nav>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        justify-content: center;
        gap: 1rem;
        background-color: gray;
        padding: 2rem;
    }

    a{
        text-decoration: none;
    }
</style>