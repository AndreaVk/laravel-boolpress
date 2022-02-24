<template>
    <div>
        <h1>{{post.title}}</h1>
        <img :src="`/storage/${post.image}`" :alt="post.title">
        <p>{{post.content}}</p>
    </div>
</template>

<script>
export default {
    name:"SinglePost",
    data(){
        return{
            post:{

            }
        }
    },
    creater(){
        axios.get('/api/posts/${this.$route.params.slug}')
        .then((response) =>{
            console.log(response.data);
        });  
    }
}
</script>

<style>

</style>