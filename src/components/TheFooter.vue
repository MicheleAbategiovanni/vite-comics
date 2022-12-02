<template>

  <footer>

    <div class="jumbotron-footer">

      <div class="p-3 container">
        <div class="row text-white">

          <div class="col-lg-4">

            <div class="row">

              <div class="col" v-for="listFooter in navMap">

                <h5>{{ listFooter.title }}</h5>
                <ul class="nav flex-column">

                  <li class="nav-item">
                    <a class="nav-link active px-0 text-secondary" href="#">{{ listFooter.listSubtitle }}</a>
                  </li>

                </ul>

              </div>

              <div class="col">DC</div>
              <div class="col">SITES</div>
              <div class="col">SHOP</div>
            </div>

          </div>

          <div class="d-none d-lg-flex col-lg-8">SPAZIO VUOTO !!!</div>

        </div>
      </div>

    </div>

    <div class="bg-secondary">
      <div class="container d-flex justify-content-between py-4">

        <div>
          <button>SIGN-UP NOW!</button>
        </div>

        <div>

          <ul class="nav justify-content-center">

            <li class="nav-item">
              <h4>FOLLOW US</h4>
            </li>

            <li class="text-white" v-for="iconList in icon">
                <img :src=iconList.src :alt=iconList.alt class="text-dark">
            </li>

          </ul>

        </div>

      </div>

    </div>

  </footer>

</template>
  
  
<script>
export default {

  data() {
    return {
      navMap: [
        {
          title: "DC COMICS",
          listSubtitle: [
            {
              list: ['1', '2'],
            }
          ],
        },
      ],
      icon: [
        {
          src:"/img/footer-facebook.png",
          alt:"logo facebook"
        },
        {
          src:"/img/footer-twitter.png",
          alt:"logo twitter"
        },
        {
          src:"/img/footer-youtube.png",
          alt:"logo youtube"
        },
        {
          src:"/img/footer-pinterest.png",
          alt:"logo pinterest"
        },
        {
          src:"/img/footer-periscope.png",
          alt:"logo periscope"
        },
      ]
    }
  }

}
</script>
  
  
  
<style lang="scss">
.jumbotron-footer {
  background-image: url("/public/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>