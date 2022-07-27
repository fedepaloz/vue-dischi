<template>
    <div class="track-card">
        <img :src="poster" :alt="title" class="img-fluid">
        <div class="title">{{title}}</div>
        <div class="author">{{author}}</div>
        <div class="year">{{year}}</div>
    </div>
</template>
 

<script>


export default{
    name: 'TrackCard',
    props:{
        poster: String,
        title: String,
        author: String, 
        year: String

    }
    }
</script>

<style lang="scss" scoped>
</style> 