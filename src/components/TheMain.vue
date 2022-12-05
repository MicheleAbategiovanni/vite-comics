<template>
    <main class="bg-dark">
        
        <!-- Container Contents -->
        <div>

            <!-- Jumbotron -->
            <div class="jumbotron py-5 text-white">
            </div>

            <!-- Container Card Comics -->
            <div class="container py-5 text-white">
                <h3> Jumbotron </h3>
            </div>

        </div>

        <!-- Container Icons -->
        <ContainerIcon></ContainerIcon>

    </main>
</template>
  
  
<script>

import ContainerIcon from './ContainerIcon.vue';

export default {
    components: {ContainerIcon},

    data() {
        return {
            text: "--> Content goes here <--",
        }
    }

}
</script>
  
  
  
<style lang="scss" scoped>
.jumbotron{
    background-image: url(/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 400px;
    background-position: top center;

    @media (max-width: 768px) {
        height: 100px;
    }
}
</style>