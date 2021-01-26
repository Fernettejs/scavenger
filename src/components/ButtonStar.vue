<template>
  <div class="button-star">
    <img class="star" id="star1" alt="star" src="../assets/star.png">
    <button @click="showStar()">Big Red Button</button>
  </div>
</template>

<script>
export default {
  name: 'ButtonStar',
  props: {
  },
  methods: {
    showStar() {
      const star1 = document.getElementById('star1');
      star1.classList.add('visible')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.button-star {
    position: relative;
}
button {
  height: 150px;
  width: 150px;
  border-radius: 100px;
  color: white;
  background: red;
  position: absolute;
  text-transform: uppercase;
  cursor: pointer;
  margin: 0;
  top: 100px;
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  box-shadow: 3px 6px #888888
}
#star1 {
  position: absolute;
  right: 100px;
  text-align: center;
}

</style>
