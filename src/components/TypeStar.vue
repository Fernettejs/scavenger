<template>
    <div class="centered">
        <input id="text" type='text' placeholder="ENTER STAR" @keyup.enter='typeStar()'/>        
        <img class="star" id="star3" alt="star" src="../assets/star.png">
    </div>
</template>

<script>
export default {
    name: 'TypeStar',
    props: {
    },
    methods: {
        typeStar() {
        const star3 = document.getElementById('star3');
        star3.classList.add('visible')

    }
}
}

</script>

<style scoped>
#text {
    background: white;
    color: black;
    position: absolute;
    margin: 0;
    top: 40%;
    left: 50%;
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    border-radius: 20px;
    text-align: center;
    padding: 10px;
}
#star3{
    position: absolute;
    margin: 0;
    top: 33%;
    left: 50%;
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}
</style>