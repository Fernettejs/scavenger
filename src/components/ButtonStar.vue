<template>
  <div class="button-star">
    <button @click="showStar()">Big Red Button</button>
    <img id="img" alt="star" src="../assets/star.png">
  </div>
</template>

<script>
export default {
  name: 'ButtonStar',
  props: {
  },
  methods: {
    showStar() {
      const img = document.getElementById('img');
      img.classList.add('visible')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  height: 200px;
  width: 200px;
  border-radius: 100px;
  color: white;
  background: red;
  position: absolute;
  left: 50px;
  bottom: 20px;
  cursor: pointer;
}

img {
  visibility: hidden;
}
.visible {
  visibility: visible;
}

</style>
