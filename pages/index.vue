<template>
  <div>
    <section class="hero__carousel">
      <div class="hero__carousel__text">
        <h3>Tortas, Cupcakes, Postres & Galletas</h3>
        <h2>Compra & Recibe en Casa</h2>
        <v-btn style="text-transform: initial;font-size: 15px;" class="mt-3" depressed color="white" :ripple="false">
          Comprar ahora
        </v-btn>
      </div>
    </section>

    <section class="mb-5">
      <h1 style="color: rgb(70,70,70);" class="text-center my-8">Shop By Category</h1>

      <v-row style="height: 310px;width: 100%;margin: 0;">
        <v-col class="first__category ml-8 mr-4">

        </v-col>

        <v-col class="second__category ml-4 mr-8">

        </v-col>
      </v-row>

      <v-row style="height: 310px;width: 100%;" class="mx-0 my-8">
        <v-col class="first__category ml-8 mr-4">

        </v-col>

        <v-col class="first__category ml-4 mr-8">

        </v-col>

        <v-col class="first__category ml-4 mr-8">

        </v-col>
      </v-row>
    </section>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Cakeland - Tortas de matrimonio, compromiso, cumpleaños y para todos tus eventos',
      meta: [{
        name: 'description',
        content: 'Mercado sin salir de casa, mercado a domicilio en Barrancabermeja.',
        hid: 'description'
      }]
    }
  },
}
</script>

<style scoped>
.hero__carousel {
  height: 690px;
  background-image: url("https://cdn.shopify.com/s/files/1/0509/8615/6220/files/Cubicake_line_up_1944x.jpg?v=1611934222");
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
  letter-spacing: 1px;
}
.hero__carousel__text {
  text-align: center;
  color: rgb(70,70,70);
}
.hero__carousel h3 {
  font-size: 20px;
}
.hero__carousel h2 {
  font-size: 30px;
  line-height: 1.4;
}
@media (max-width: 1400px) and (min-width: 1000px) {
  .hero__carousel {
    height: 500px;
  }
}
@media (max-width: 999px) and (min-width: 0) {
  .hero__carousel {
    height: 350px;
  }
}
.first__category {
  background-image: url("https://cdn.shopify.com/s/files/1/0509/8615/6220/collections/Evoke_20Pictures_20Lifestyle_Creative_20Shoot_80_900x.jpg?v=1611936089");
  background-size: auto;
  background-position: center;
}
.second__category {
  background-image: url("https://cdn.shopify.com/s/files/1/0509/8615/6220/collections/DSC08982_900x.jpg?v=1618498382");
  background-size: auto;
  background-position: center;
}
</style>
