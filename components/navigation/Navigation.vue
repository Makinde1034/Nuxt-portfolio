<template>
    
    <nav class="nav">
        <h3>Tolulope</h3>
        <ul>
            <nuxt-link style="marginRight:30px" to="/">Home</nuxt-link>
            <nuxt-link style="marginRight:30px" to="projects" >Projects</nuxt-link>
            <a href="linkedin">LinkedIn</a>
        </ul>
    </nav>    
    
</template>

<script>
export default {
    data(){
        return{
            linkedin:"linkedin.com/in/tolu-makinde-20a886108"
        }
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Ms+Madi&display=swap');

.wrap{
    display: flex;
    flex-direction: column;
    align-items: center;
    
}
.nav{
    color: white;
    height: 60px;
    display: flex; 
    align-items: center;
    justify-content: space-between;
    padding: 0px 20px 0px 20px;
}

.nav h3{
    font-family: 'Ms Madi', cursive;
    /* color: #f2de63; */
}

.nav ul{
    display: flex;
    align-items: center;
    list-style: none;
}

.nav ul a{
    font-size: 12px;
    text-decoration: none;
    color: white;
    font-family: 'Work Sans', sans-serif;
}

.nav ul a:hover{
    color: #f2de63;
}
</style>