<script setup>

const props = defineProps({
  version: Number,
  title: String,
  typeFile: String,
  sizeFile: String,
  date: String,
  url: String
})

</script>


<template>
    <main class="file-box">
        <h1>VERSION {{props.version}}</h1>
        <h3>{{ props.title }}</h3>

        <section class="file-content">
            <p>{{ props.typeFile }}</p>
            <p> /{{ props.sizeFile }}</p>
            <span> <p>{{ props.date }}</p><img src="../assets/img/download.svg" alt="" /></span>
            
        </section>
    </main>

</template>

<style>
.file-box{
    display: flex;
    flex-direction: column;
    position: relative;
    border-bottom: 0.3px solid black;
    border-top: 0.3px solid black;
    height: 6rem;
    padding-bottom: 2rem;
}

h1{
   font-size: 1rem; 
}

h3{
    font-size: 0.8rem;
}

.file-content{
    display: flex;
    flex-direction: row;
    column-gap: 0.5rem;
    font-size: 0.8rem;
}


.file-content img{
    width: 1.5rem;
    height: 1.5rem;
    position: absolute;
    right: 2rem;
    bottom: 3.5rem;
}

</style>