<template>

  <header>

    <nav class="navbar navbar-expand-lg bg-light py-3">
      
      <div class="container">
        
        <div>
          <a class="navbar-brand" href="#">
            <img src="/img/dc-logo.png" alt="logo dc comics">
          </a>
        </div>

        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="d-none d-lg-flex">

          <ul class="navbar-nav">

            <li class="nav-item" v-for="(navItem) in items">
              <a class="nav-link active fs-6" aria-current="page" href="#">{{ navItem.title }}</a>
            </li>

          </ul>

        </div>

      </div>

    </nav>

  </header>

</template>


<script>
export default {

  data() {
    return {
      items: [
        {
          title: "CHARACTERS",
        },
        {
          title: "COMICS",
        },
        {
          title: "MOVIES",
        },
        {
          title: "TV",
        },
        {
          title: "GAMES",
        },
        {
          title: "COLLECTIBLES",
        },
        {
          title: "VIDEOS",
        },
        {
          title: "FANS",
        },
        {
          title: "NEWS",
        },
        {
          title: "SHOP",
        },
      ]
    }
  }

}
</script>



<style lang="scss">


</style>