<script>
import Navbar from "@/components/navbar";
import Service from "@/components/services";
import Features from "@/components/features";
import Pricing from "@/components/pricing";
import Blog from "@/components/blog";
import Contact from "@/components/contact";
import Footer from "@/components/footer";

/**
 * Index-1
 */
export default {
  components: { Navbar, Service, Features, Pricing, Blog, Contact, Footer }
};
</script>

<template>
  <div>
    <Navbar />
    <div v-scroll-spy>
      <!-- Hero Start -->
      <section
        class="hero-1-bg"
        :style="{'background-color': '#3a7a48'}"
        id="home"
      >
        <div class="container">
          <div class="row align-items-center justify-content-center">
            <div class="col-lg-6">
              <h1
                class="hero-1-title text-light font-weight-bold text-shadow mb-4"
              >Gagnez en efficacité et en flexibilité.</h1>
              <div class="w-75 mb-5 mb-lg-0">
                <p class="text-light mb-5 pb-5 font-size-17">
                  Notre suite d'outils est la pour aider les acteurs de la transition énergétique dans leurs processus administratifs & marketings.
                </p>
                <div class="subscribe-form">
                  <form action="#">
                    <input type="text" placeholder="Votre email professionel..." />
                    <button type="submit" class="btn btn-primary">Lancez-vous!</button>
                  </form>
                </div>
              </div>
            </div>
            <div class="col-lg-6 col-md-10">
              <div class="mt-5 mt-lg-0">
                <img src="@/assets/images/undraw_data_processing_yrrv.svg" alt class="img-fluid d-block mx-auto" />
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- Hero End -->
      <Service />
      <Features />
      <!-- <Pricing />
      <Blog /> -->
      <Contact />
      <Footer />
    </div>
  </div>
</template>