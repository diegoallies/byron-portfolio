<template>
  <div class="home" id="index">
    <div class="container">
      <div class="row">
        <div class="col-sm w3-animate-right">
          <!-- Left Column -->
          <div class="imageContainer">
            <img
              src="https://i.postimg.cc/fyHXWg56/4-EE856-A8-BBE1-48-BD-B2-CD-DA43-D2-AE88-A7.jpg"
              alt="Byron Moses"
              class="home-image"
            />
          </div>
        </div>
        <div class="col-sm w3-animate-left">
          <!-- Right Column -->
          <h1><HelloWorld msg="I am Byron Moses" /></h1>
        </div>
      </div>
    </div>
  </div>
  <Footer />
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    Footer,
  },
};
</script>

<style scoped>
.imageContainer {
  width: 85%;
  height: 100%;
  margin-left: -5%;
}

.home-image {
  width: 100%;
  height: 100%;
}

/* media querries */

@media only screen and (max-width: 553px) {
  .home-image {
    margin-top: 15%;
    margin-bottom: 15%;
    margin-left: 15%;
    margin-right: -5%;
  }

  .col-sm {
    margin-left: 0%;
    margin-right: 0%;
  }


}
</style>
