<template>
  <div>
    <TheHeader></TheHeader>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
export default{
  name:'App',
  components:{
    TheHeader,
    
}
}
</script>

<style lang="scss">
@import './assets/scss/style.scss';
</style>
