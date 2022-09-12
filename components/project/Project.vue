<template>
    <div class="project" >
        <h3>{{title}}</h3>
        <p class="project__tools">{{tools}}</p>
        <p class="project__about">{{about}}</p>
        <span>
            <a style="color:#f2de63;text-decoration: underline;" :href="site">Site</a>
            <a v-if="frontendrepo" :href="frontendrepo">Repo (Frontend)</a>
            <a v-if="backendrepo" :href="backendrepo">Repo (Backend)</a>
        </span>
    </div>
</template>

<script>
export default {
    
    props: {
        title: {
            type: String,
            default : ""
        },
        about: {
            type : String,
            default : ""
        },
        tools: {
            type : String,
            default : ""
        },
        frontendrepo: {
            type : String,
            default : ""
        },
        backendrepo: {
            type : String,
            default : ""
        },
        site: {
            type : String,
            default : ""
        }
        
        
    }
}
</script>

<style scoped >

@import url('https://fonts.googleapis.com/css2?family=Work+Sans&display=swap');



.project{
    /* height: 200px; */
    padding: 20px;
    border: 1px solid white;
    border-radius: 5px; 
    font-family: 'Work Sans', sans-serif;
    transition: 0.3s ease-in-out;
    width: 100%;
    /* background: red; */
}

.project:hover{
    /* border: 1px solid #f2de63; */
    cursor: pointer;
}

.project h3{
   margin-bottom: 10px;
}



.project__tools,.project__about{
    font-size: 12px;
    margin-bottom: 10px;
    line-height: 20px;
}

.project span{
    display: flex;
    flex-direction: column;
    /* align-items: center; */
}

.project span a{
    margin-bottom: 10px;
    font-size: 12px;
    color: white;
    
}

#site{
    color: #f2de63;
}

@media screen and (max-width:768px)  {
    
}
</style>