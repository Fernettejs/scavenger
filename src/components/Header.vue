<template>
    <header class="header">
        <h1 class="centered">Star Scavenger Hunt</h1>
        <h3 class="centered">Find all 3 <span @mouseover="hoverToggle()" id="text">stars</span> to win!</h3>
        <img class="star centered" id="star2" alt="star" src="../assets/star.png">
    </header>
</template>

<script>
import ButtonStar from './ButtonStar.vue'

export default {
    name: "Header",
    components: {
        ButtonStar
    },
      methods: {
    hoverToggle() {
      const star2 = document.getElementById('star2');
      star2.classList.add('visible')
    }
  }
}
</script>

<style scoped>

span:hover {
cursor: pointer;

}
#star2 {
  position: absolute;
  left: 100px;
  text-align: center;
}
</style>