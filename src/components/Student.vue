<script setup>

const props = defineProps({
  img: String,
  content: String
})

</script>



<template>
<div class="st-msg">
    <section class="bubble-box">
        <p>{{ props.content }}</p>
    </section>
    <img src="props.img" alt="">
</div>
</template>

<style >
.st-msg{
    display: flex;
    flex-direction: row;   
    align-items: center;
    width: 100%;
    position: absolute;
}

.st-msg img{
    border-radius: 50%;
    height: 2rem;
    width: 2rem;
    position: absolute;
    right: 1rem;
}

.bubble-box{
    width: 70%;
    right: 4rem;
    display: flex;
    justify-content: center;
    padding: 10px;
    position: absolute;
    border-radius: 8px 8px 8px 8px;
    border: 1px solid black;
}


</style>