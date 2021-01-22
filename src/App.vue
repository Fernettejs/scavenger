<template>
  <ButtonStar />
</template>

<script>
import ButtonStar from './components/ButtonStar.vue'

export default {
  name: 'App',
  components: {
    ButtonStar
  }
}
</script>

<style>
* {
 box-sizing: border-box;
 margin: 0;
 padding: 0;
}
 
body {
 font-family: Arial, Helvetica, sans-serif;
 line-height: 1.4;
}

</style>
