<template>
    <main class="bg-dark">
        
        <!-- Container Contents -->
        <div>

            <div class="container py-5 text-white">
                <h3> {{ text }} </h3>
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
  
  
  
<style lang="scss">

</style>