<template>
  <v-container>
    <nav id="mynav">
    <v-row>
     
      <v-col cols="2" id="iconcol" style="">
        
          <v-app-bar-nav-icon
            ><svg
              width="50"
              height="50"
              viewBox="0 0 100 100"
              fill="orange"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M20.8458 19.4166C20.8458 13.1832 25.9749 7.73325 32.5999 8.38741C54.172 10.5237 74.158 20.6743 88.6083 36.8332C93.0666 41.8041 91.6791 49.1832 86.6124 52.8541L84.8499 54.1332L83.3374 51.8832L83.3041 51.8374C70.0124 33.4749 48.3874 21.5249 23.9708 21.5249H20.8458V19.4166ZM78.2124 55.4582L79.7874 57.8041L63.3416 69.7416L62.4999 70.3666V79.1249C62.4999 80.23 62.0609 81.2898 61.2795 82.0712C60.4981 82.8526 59.4383 83.2916 58.3333 83.2916C57.2282 83.2916 56.1684 82.8526 55.387 82.0712C54.6056 81.2898 54.1666 80.23 54.1666 79.1249V78.8749C54.0999 78.3505 53.8364 77.871 53.4294 77.5336C53.0224 77.1963 52.5023 77.0262 51.9746 77.058C51.4469 77.0898 50.951 77.321 50.5875 77.7048C50.2239 78.0886 50.0198 78.5963 50.0166 79.1249V85.3791C50.0167 86.4481 49.6059 87.4763 48.8692 88.251C48.1325 89.0257 47.1262 89.4875 46.0585 89.541C44.9908 89.5946 43.9434 89.2356 43.1329 88.5385C42.3224 87.8414 41.8109 86.8594 41.7041 85.7957L35.7041 90.1291C29.4999 94.6041 20.8291 90.1749 20.8333 82.5207L20.8458 27.7707H23.9708C46.2791 27.7707 66.0374 38.6749 78.2124 55.4582ZM37.5166 45.7916C38.6217 45.7916 39.6815 45.3526 40.4629 44.5712C41.2443 43.7898 41.6833 42.73 41.6833 41.6249C41.6833 40.5198 41.2443 39.46 40.4629 38.6786C39.6815 37.8972 38.6217 37.4582 37.5166 37.4582C36.4115 37.4582 35.3517 37.8972 34.5703 38.6786C33.7889 39.46 33.3499 40.5198 33.3499 41.6249C33.3499 42.73 33.7889 43.7898 34.5703 44.5712C35.3517 45.3526 36.4115 45.7916 37.5166 45.7916ZM54.1832 58.2832C55.2883 58.2832 56.3481 57.8443 57.1295 57.0629C57.9109 56.2815 58.3499 55.2216 58.3499 54.1166C58.3499 53.0115 57.9109 51.9517 57.1295 51.1703C56.3481 50.3889 55.2883 49.9499 54.1832 49.9499C53.0782 49.9499 52.0184 50.3889 51.237 51.1703C50.4556 51.9517 50.0166 53.0115 50.0166 54.1166C50.0166 55.2216 50.4556 56.2815 51.237 57.0629C52.0184 57.8443 53.0782 58.2832 54.1832 58.2832ZM37.5166 70.7749C38.6217 70.7749 39.6815 70.3359 40.4629 69.5545C41.2443 68.7731 41.6833 67.7133 41.6833 66.6082C41.6833 65.5032 41.2443 64.4434 40.4629 63.662C39.6815 62.8806 38.6217 62.4416 37.5166 62.4416C36.4115 62.4416 35.3517 62.8806 34.5703 63.662C33.7889 64.4434 33.3499 65.5032 33.3499 66.6082C33.3499 67.7133 33.7889 68.7731 34.5703 69.5545C35.3517 70.3359 36.4115 70.7749 37.5166 70.7749Z"
                fill="orange"
              />
            </svg>
          </v-app-bar-nav-icon>
          <v-col cols="2" style="position: relative;">
        <h3>pizza</h3>
      </v-col>
      </v-col>
      
      <v-col style="display: flex;align-self: center;" cols="10">
        <v-row id="linkscon" 
          ><v-col
            style="width: fit-content"
            v-for="(link, i) in links"
            :key="i"
          >
            <nuxt-link :to="link.url" style="text-decoration: none">{{
              link.linkname
            }}</nuxt-link>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  
  </nav>
  </v-container>
  
  <slot></slot>

</template>

<script>
export default {
  data() {
    return {
      links: [
        { linkname: "home", url: "#homeBaaner" },
        { linkname: "about", url: "#about" },
        { linkname: "proudect", url: "#proudect" },
        { linkname: "location", url: "#location" },
        { linkname: "order", url: "#order" },
      ],
    };
  },
};
</script>

<style scoped>
a:active {
  color: rgb(255, 0, 0);
}
a:link {
  color: orange;
}
a:not(:active) {
  color: rgb(240, 165, 4);
}
#linkscon {
  position: relative;
  width: fit-content;
}
#iconcol {
display: flex;
}
/*/labtop/*/
@media (max-width: 1366px) {
}
/*/tablet/*/
@media (max-width: 991px) {
}
/*/mobile/*/
@media (max-width: 500px) {
  #iconcol {
display: flex;
flex-flow: column;
align-items: center;
justify-content: center;
text-align: center;
}
#iconcol h3 {
position: relative;
left: -20px;
}
}
</style>
