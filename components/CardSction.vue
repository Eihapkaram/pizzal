<template>
  <v-lazy
    :min-height="200"
    :options="{ threshold: 0.5 }"
    transition="fade-transition"
  >
    <v-container
      style="height: fit-content; width: 100%; position: relative"
      id="proudect"
      class="cardcon"
    >
      <v-row>
        <v-col cols="12" id="header" style="text-align: center">
          <h2
            style="font-size: large"
            data-aos="fade-out"
            data-aos-duration="1700"
          >
            The Most Discovred Pizzas
          </h2>
          <p data-aos="fade-out" data-aos-duration="1900" class="subtitle-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non
          </p>
        </v-col></v-row
      >

      <v-row
        style="
          gap: 20px;
          display: flex;
          flex-flow: row, wrap;
          justify-content: center;
          height: fit-content;
        "
      >
        <v-card
          data-tilt
          data-tilt-reset="true"
          data-aos="fade-out"
          data-aos-duration="1000"
          class="card"
          elevation="3"
          style="top: 100px; position: relative"
          max-width="300"
        >
          <div id="inner">
            <v-img
              class="align-end text-white mx-auto"
              height="100px"
              width="100px"
              style="position: relative"
              src="/public/img/product-1.png"
              cover
            >
            </v-img>
          </div>

          <v-card-title style="text-align: center"
            >marshmalow</v-card-title
          >

          <v-card-subtitle class="pt-4"> $10 </v-card-subtitle>

          <v-card-text>
            <div>Whitehaven Beach</div>

            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">show-detilse</v-btn>

            <v-btn color="orange">order<v-icon>mdi-cart</v-icon></v-btn>
          </v-card-actions>
        </v-card>
        <v-card
          data-aos="fade-out"
          data-aos-duration="1200"
          data-tilt
          data-tilt-reset="true"
          elevation="3"
          style="top: 100px; position: relative"
          max-width="300"
        >
          <v-img
            class="align-end text-white mx-auto"
            height="100px"
            width="100px"
            style="position: relative"
            src="/public/img/product-5.png"
            cover
          >
          </v-img>
          <v-card-title style="text-align: center">New-York</v-card-title>

          <v-card-subtitle class="pt-4"> $10 </v-card-subtitle>

          <v-card-text>
            <div>Whitehaven Beach</div>

            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">show-detilse</v-btn>

            <v-btn color="orange">order<v-icon>mdi-cart</v-icon></v-btn>
          </v-card-actions>
        </v-card>
        <v-card
          data-aos="fade-out"
          data-aos-duration="1300"
          data-tilt
          data-tilt-reset="true"
          elevation="3"
          style="top: 100px; position: relative"
          max-width="300"
        >
          <v-img
            class="align-end text-white mx-auto"
            height="100px"
            width="100px"
            style="position: relative"
            src="/public/img/product-1.png"
            cover
          >
          </v-img>
          <v-card-title style="text-align: center"
            >marshmalow</v-card-title
          >

          <v-card-subtitle class="pt-4"> $8 </v-card-subtitle>

          <v-card-text>
            <div>Whitehaven Beach</div>

            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">show-detilse</v-btn>

            <v-btn color="orange">order<v-icon>mdi-cart</v-icon></v-btn>
          </v-card-actions>
        </v-card>
        <v-card
          data-aos="fade-out"
          data-aos-duration="1400"
          data-tilt
          data-tilt-reset="true"
          elevation="3"
          style="top: 100px; position: relative"
          max-width="300"
        >
          <v-img
            class="align-end text-white mx-auto"
            height="100px"
            width="100px"
            style="position: relative"
            src="/public/img/product-2.png"
            cover
          >
          </v-img>
          <v-card-title style="text-align: center">meet</v-card-title>

          <v-card-subtitle class="pt-4"> $16 </v-card-subtitle>

          <v-card-text>
            <div>Whitehaven Beach</div>

            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">show-detilse</v-btn>

            <v-btn color="orange">order<v-icon>mdi-cart</v-icon></v-btn>
          </v-card-actions>
        </v-card>
        <v-card
          data-aos="fade-out"
          data-aos-duration="1500"
          data-tilt
          data-tilt-reset="true"
          elevation="3"
          style="top: 100px; position: relative"
          max-width="300"
        >
          <v-img
            class="align-end text-white mx-auto"
            height="100px"
            width="100px"
            style="position: relative"
            src="/public/img/product-3.png"
            cover
          >
          </v-img>
          <v-card-title style="text-align: center"
            >mogzrilla</v-card-title
          >

          <v-card-subtitle class="pt-4"> $20 </v-card-subtitle>

          <v-card-text>
            <div>Whitehaven Beach</div>

            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">show-detilse</v-btn>

            <v-btn color="orange">order<v-icon>mdi-cart</v-icon></v-btn>
          </v-card-actions>
        </v-card>
        <v-card
          data-aos="fade-out"
          data-aos-duration="1600"
          data-tilt
          data-tilt-reset="true"
          elevation="3"
          style="top: 100px; position: relative"
          max-width="300"
        >
          <v-img
            class="align-end text-white mx-auto"
            height="100px"
            width="100px"
            style="position: relative"
            src="/public/img/product-4.png"
            cover
          >
          </v-img>
          <v-card-title style="text-align: center">furuts</v-card-title>

          <v-card-subtitle class="pt-4"> $15 </v-card-subtitle>

          <v-card-text>
            <div>Whitehaven Beach</div>

            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">show-detilse</v-btn>

            <v-btn color="orange">order<v-icon>mdi-cart</v-icon></v-btn>
          </v-card-actions>
        </v-card>
      </v-row>
    </v-container>
  </v-lazy>
</template>

<script>
import VanillaTilt from "vanilla-tilt";
export default {
  //@click="$router.push({ name: 'id', params: { id: 1 } })"
  async mounted() {
    const element = "null";
    VanillaTilt.init(element.value, { max: 20, speed: 400 });
  },
};
</script>

<style scoped>
.cardcon {
  margin-bottom: 300px;
}
#header {
  margin: 0px;
}
/*/tablet/*/
@media (max-width: 991px) {
  .cardcon {
    margin-bottom: 200px;
  }
}
/*/mobile/*/
@media (max-width: 500px) {
}
.card {
  transform-style: preserve-3d;
  transform: perspective(1000px);
}
#inner {
  transform: translateZ(20px);
}
</style>
