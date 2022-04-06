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
      <h1 style="color: rgb(70,70,70);" class="text-center my-9">Compra por Categoría</h1>

      <v-row style="height: 310px;width: 100%;margin: 0;padding: 0 32px;">
        <v-col class="shop__by__category__category first__category mr-4">
          <h2 class="category__title">Tortas para Ocasiones</h2>
        </v-col>

        <v-col class="shop__by__category__category second__category ml-4">
          <h2 class="category__title">Postres & Dulces</h2>
        </v-col>
      </v-row>

      <v-row style="height: 310px;width: 100%;padding: 0 32px;" class="mx-0 my-8">
        <v-col class="shop__by__category__category first__category mr-4">
          <h2 class="category__title">Tortas para Dos</h2>
        </v-col>

        <v-col class="shop__by__category__category first__category ml-4">
          <h2 class="category__title">Cupcakes y Chessecakes</h2>
        </v-col>

        <v-col class="shop__by__category__category first__category ml-8">
          <h2 class="category__title">Galletas</h2>
        </v-col>
      </v-row>
    </section>

    <h2 style="color: rgb(70,70,70);" class="text-center my-9">Productos Populares</h2>
    <v-row style="width: 100%;margin: 0;">
      <div class="popular__products__grid">
        <div class="popular__products__card" v-for="n in dummyProducts">
          <v-img :src="n.image" alt="" class="popular__products__card__image" contain />
          <div class="popular__products__card__info">
            <p class="popular__products__card__info__title">{{ n.title }}</p>
            <h4 class="popular__products__card__price">{{ n.price | currency }}</h4>
          </div>
        </div>
      </div>
    </v-row>
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
  data() {
    return {
      dummyProducts: [
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC08332_1_590x.jpg?v=1618919651',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        },
        {
          title: 'Caja de chocolates negros',
          image: 'https://cdn.shopify.com/s/files/1/0509/8615/6220/products/DSC07684_590x.jpg?v=1612457733',
          price: 25000
        }
      ]
    }
  }
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
  color: rgb(70, 70, 70);
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
  display: flex;
  justify-content: center;
  align-items: center;
}

.second__category {
  background-image: url("https://cdn.shopify.com/s/files/1/0509/8615/6220/collections/DSC08982_900x.jpg?v=1618498382");
  background-size: auto;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.category__title {
  text-align: center;
  color: rgb(70, 70, 70);
  padding: 2px 6px;
  background-color: rgba(250,250,250,0.7);
  border-radius: 10px;
}

.popular__products__grid {
  display: grid;
  grid-template-columns: repeat(auto-fill,[col-start] minmax(500px,1fr) [col-end]);
  grid-gap: 15px;
  padding: 0 32px;
  width: 100%;
}

.popular__products__card {
  height: 410px;
}

.popular__products__card__image {
  width: auto;
  min-height: 350px;
  max-height: 350px;
}

.popular__products__card__info {
  text-align: center;
}

.popular__products__card__info__title {
  margin: 10px 0 0;
  font-size: 17px;
}
</style>
