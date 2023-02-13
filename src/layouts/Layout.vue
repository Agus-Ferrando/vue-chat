<script setup>
import File from "../components/File.vue"
import Professor from "../components/Professor.vue"
import Student from "../components/Student.vue"


</script>

<template>
    <body>
        <header>
            <h2>Comentarios</h2><img src="../assets/img/close.svg" alt="" />
        </header>

        <main>
            <File 
                version="1"
                title="file.pdf"
                type-file="Documento/PDF"
                size-file="3.8MB"
                date="28 dic 2018"
                class="file"
            />

            <Professor 
                img="../assets/img/person.svg"
                content="hi"
                class="professor"
            />

            <Student 
                img="../assets/img/person.svg"
                content="hello"
                class="student"
            />

        </main>

        <footer>
            <input type="text" /><img src="../assets/img/send.svg" alt="" />
        </footer>

    </body>
</template>

<style>
body{
    display: flex;
    flex-direction: column;
    box-sizing: border-box;
    margin: 0;
}

header{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    column-gap: 3rem;
}

header img{
    height: 1rem;
    width: 1rem;
    position: absolute;
    right: 1rem;
}

footer{
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    column-gap: 1rem;
    position: absolute;
    bottom: 5rem;
}

footer input{
    width: 300px;
    height: 5rem;
}

footer img {
    height: 1.5rem;
    width: 1.5rem;
}

.professor{
    margin-top: 3rem;
}

.student{
    position: absolute;
    margin-top: 6rem;
}
</style>