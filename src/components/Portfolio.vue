<template>
  <section class="page-section bg-light" id="portfolio">
      <div class="container">
          <div class="text-center">
              <h2 class="section-heading text-uppercase">Portfolio</h2>
              <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
          </div>
          <div class="row">
              <div class="col-lg-4 col-sm-6 mb-4" v-for="(obj, key) in portfolioJson" :key="key">
                  <!-- Portfolio item 1-->
                  <div class="portfolio-item">
                      <a class="portfolio-link" data-bs-toggle="modal" href="#portfolioModal1">
                          <div class="portfolio-hover">
                              <div class="portfolio-hover-content"><i class="fas fa-plus fa-3x"></i></div>
                          </div>
                          <img class="img-fluid" src="assets/img/portfolio/1.jpg" alt="..." />
                      </a>
                      <div class="portfolio-caption">
                          <div class="portfolio-caption-heading">{{obj.title}}</div>
                          <div class="portfolio-caption-subheading text-muted">{{obj.title}}</div>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </section>
    
</template>

<script>
export default {
    data: () => ({
        portfolioJson: [
            {
                img: "/something/random/img.jpg",
                caption: "Explore",
                title: "Graphic Design"
            },
            {
                img: "/something/random/img.jpg",
                caption: "Finish",
                title: "Identity"
            },
            {
                img: "/something/random/img.jpg",
                caption: "Lines",
                title: "Branding"
            },
            {
                img: "/something/random/img.jpg",
                caption: "Southwest",
                title: "Website Design"
            },
            {
                img: "/something/random/img.jpg",
                caption: "Window",
                title: "Photography"
            },
            {
                img: "/something/random/img.jpg",
                caption: "Coffee",
                title: "Drink a Lot!"
            }
        ]
    })
}
</script>

<style lang="sass">

</style>