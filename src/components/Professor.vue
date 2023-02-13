<script setup>

const props = defineProps({
  img: String,
  content: String
})

</script>



<template>
<div class="prof-msg">
    <img src="props.img" alt="">
    <section class="bubble">
        <p>{{ props.content }}</p>
    </section>
</div>
</template>

<style >
.prof-msg{
    display: flex;
    flex-direction: row;   
    align-items: center;
    width: 100%;
}

.prof-msg img{
    border-radius: 50%;
    height: 2rem;
    width: 2rem;
    position: absolute;
    left: 1rem;
}

.bubble{
    width: 70%;
    margin-left: 4rem;
    display: flex;
    justify-content: center;
    padding: 10px;
    position: absolute;
    border-radius: 8px 8px 8px 8px;
    border: 1px solid black;
}


</style>