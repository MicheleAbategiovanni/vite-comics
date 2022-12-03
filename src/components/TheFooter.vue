<template>

  <footer>

    <!-- Nav Footer -->
    <div class="jumbotron-footer">

      <div class="p-3 container">
        <div class="row row-cols-3 text-white">

          <div class="col">

            <div class="row row-cols-3">

              <div class="col" v-for="listFooter in navMap">

                <h5>{{ listFooter.title }}</h5>
                <ul class="nav flex-column">

                  <li class="nav-item">
                    <a class="nav-link active px-0 text-secondary" href="#">{{ listFooter.listSubtitle }}</a>
                  </li>

                </ul>

              </div>

            </div>

          </div>

          <div class="d-none d-lg-flex col-lg-8">SPAZIO VUOTO !!!</div>

        </div>
      </div>

    </div>

    <!-- Social Nav -->
    <div class="bg-footer">

      <div class="container d-flex justify-content-between py-4">

        <!-- Container Button -->
        <div>
          <button type="button" class="border-blue text-white p-3 ">SIGN-UP NOW!</button>
        </div>

        <!-- Container Icon Social -->
        <div>

          <ul class="nav align-items-center">

            <li class="nav-item">
              <a class="nav-link px-2 fw-bold fs-5" href="#">FOLLOW US
              </a>
            </li>

            <li class="text-white" v-for="iconList in icon">
              <a class="nav-link px-2" href="#">
                <img :src=iconList.src :alt=iconList.alt class="text-dark">
              </a>
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
        {
          title: "DC",
          listSubtitle: [
            {
              list: ['1', '2'],
            }
          ],
        },
        {
          title: "SITES",
          listSubtitle: [
            {
              list: ['1', '2'],
            }
          ],
        },
        {
          title: "SHOP",
          listSubtitle: [
            {
              list: ['1', '2'],
            }
          ],
        },
      ],
      icon: [
        {
          src: "/img/footer-facebook.png",
          alt: "logo facebook"
        },
        {
          src: "/img/footer-twitter.png",
          alt: "logo twitter"
        },
        {
          src: "/img/footer-youtube.png",
          alt: "logo youtube"
        },
        {
          src: "/img/footer-pinterest.png",
          alt: "logo pinterest"
        },
        {
          src: "/img/footer-periscope.png",
          alt: "logo periscope"
        },
      ]
    }
  }

}
</script>
  
  
  
<style lang="scss">
.jumbotron-footer {
  background-image: url("/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.bg-footer {
  background-color: #303030;
}

.border-blue {
  border: 3px solid #0282F9;
  background-color: transparent;
  font-weight: bold;
}
</style>