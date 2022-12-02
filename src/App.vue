<template>

<TheHeader></TheHeader>

<TheMain></TheMain>

<TheFooter></TheFooter>

</template>


<script>

import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  components: {TheHeader, TheMain , TheFooter}

}
</script>



<style lang="scss">
@use "./styles/general.scss";



</style>