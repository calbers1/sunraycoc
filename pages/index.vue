<template>
  <span>
    <MainHeader></MainHeader>
    <NuxtLink to="/Home">Home Page</NuxtLink>
  </span>
  </template>

<script>
import MainHeader from '~/components/MainHeader.vue';
export default {
    name: "IndexPage",
    components: { MainHeader }
}
</script>


<style lang="scss">
  .main-content{
    padding-inline: 40px;

    @media only screen and (max-width: 992px){
      padding-inline: 20px;
    }
  }
</style>
