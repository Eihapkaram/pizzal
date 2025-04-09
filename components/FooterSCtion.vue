<template>
  <v-container style="width: 97%">
    <v-row style="text-align: center">
      <v-col style="margin-left: auto; position: relative" cols="12" lg="12"
        ><h3 style="font-size: medium">pizza</h3>
        <img src="/public/img/logo-pizza.svg" />
        <br />
        <v-row id="bigconrow" style="">
          <v-col cols="5"
            ><h3 style="font-size: medium">social</h3>
            <v-row
              style="margin-top: 20px; position: relative; left: 40%; gap: 20px"
            >
              <v-icon style="cursor: pointer">mdi-facebook</v-icon>
              <v-icon style="cursor: pointer">mdi-instagram</v-icon>
              <v-icon style="cursor: pointer">mdi-twitter</v-icon>
            </v-row>
          </v-col>

          <v-col cols="4" style="position: relative"
            ><h3 style="font-size: medium">subscribe for Discounts</h3>
            <v-btn
              @click="fun1()"
              id="mybtn"
              elevation="3"
              style="border-radius: 30px"
              >sebscribe
            </v-btn>
          </v-col>
          <v-col id="payment" cols="4" style=""
            ><h3 style="font-size: medium">payment methods</h3>

            <v-row id="paymentimg" style="">
              <img src="/public/img/footer-card-1.png" />
              <img src="/public/img/footer-card-2.png" />
              <img src="/public/img/footer-card-3.png" />
              <img src="/public/img/footer-card-4.png" />
            </v-row>
          </v-col>
        </v-row>
      </v-col>
      <v-col style="margin-left: auto; position: relative" cols="12" lg="12"
        ><h3 style="font-size: medium">All righets reseved by Eihap karam</h3>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      active: false,
    };
  },
  methods: {
    fun1() {
      if (this.active == false) {
        window.mybtn.style.color = "red";
        window.mybtn.innerHTML = "sebscrped";
        this.active = true;
      } else {
        window.mybtn.style.color = "black";
        window.mybtn.textContent = "sebscrpe";
        this.active = false;
      }
    },
  },
};
</script>
<style>
#payment {
  align-items: center;
}
#paymentimg {
  position: relative;
  left: 10%;
  gap: 20px;
  top: 20px;
}
#bigconrow {
  margin-left: auto;
  position: relative;
  display: flex;
  flex-flow: row nowrap;
  left: -10%;
}
/*/tablet/*/
@media (max-width: 991px) {
}
/*/mobile/*/
@media (max-width: 500px) {
  #payment {
    display: flex;
    position: relative;
    flex-flow: column;
    align-items: center;
    margin-bottom: 40px;
  }
  #paymentimg img {
    position: relative;
    display: flex;
    flex-flow: column, wrap;
    width: 40px;
  }
  #bigconrow {
    position: relative;
    display: flex;
    flex-flow: row nowrap;
  }
}
</style>
