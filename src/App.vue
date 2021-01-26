<template>
  <Header />
  <ButtonStar />
  <TypeStar />

</template>

<script>
import Header from './components/Header.vue'
import ButtonStar from './components/ButtonStar.vue'
import TypeStar from './components/TypeStar.vue'

export default {
  name: 'App',
  components: {
    Header,
    ButtonStar,
    TypeStar
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
 background: #c0c0c0;
}
.centered {
  text-align: center;

}
.star {
  height: 65px;
  display: flex;
}
img {
  visibility: hidden;
}
.visible {
  visibility: visible;
}

</style>
