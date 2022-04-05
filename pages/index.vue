<template>
  <div>
    <section class="main-banner">
    </section>

    <section class="">
      <h1 class="text-center my-8">Shop By Category</h1>

      <v-row style="height: 310px;width: 100%;margin: 0;">
        <v-col class="first__category ml-4 mr-2">

        </v-col>
        <v-col class="first__category ml-2 mr-4">

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
.main-banner {
  height: 690px;
  background-image: url("https://cdn.shopify.com/s/files/1/0509/8615/6220/files/Cubicake_line_up_1944x.jpg?v=1611934222");
  background-size: cover;
  background-position: center;
}
@media (max-width: 1400px) and (min-width: 1000px) {
  .main-banner {
    height: 500px;
  }
}
@media (max-width: 999px) and (min-width: 0) {
  .main-banner {
    height: 350px;
  }
}
.first__category {
  background-image: url("https://cdn.shopify.com/s/files/1/0509/8615/6220/collections/Evoke_20Pictures_20Lifestyle_Creative_20Shoot_80_900x.jpg?v=1611936089");
  background-size: auto;
  background-position: center;
}
</style>
