<template>
  <v-app>
    <header class="header">
      <p class="header__text">Envíos gratis desde $55.000</p>
    </header>
    <nav class="navbar">
      <div class="nav__wrapper">
        <v-icon
          size="29"
          class="nav__wrapper__icon"
          color="rgb(90,90,90)"
        >mdi-menu
        </v-icon>
      </div>
      <div class="navbar__logo">
        <img class="navbar__logo__image"
             src="https://firebasestorage.googleapis.com/v0/b/real-web-project.appspot.com/o/Cake%20shop%20(1).png?alt=media&token=40ccd33d-4c1f-47d0-a2f7-ab36706bc9b8"
             alt="">
      </div>
      <div class="navbar__actions">
        <v-icon size="29" color="rgb(90,90,90)" class="navbar__actions__icon">mdi-account</v-icon>
        <v-icon size="29" color="rgb(90,90,90)" class="navbar__actions__icon">mdi-magnify</v-icon>
        <v-icon size="29" color="rgb(90,90,90)" class="navbar__actions__icon">mdi-cart</v-icon>
      </div>
    </nav>
    <nuxt/>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
        },
      ],
    }
  },
}
</script>

<style scoped>
.header {
  display: flex;
  height: 35px;
  background-color: sandybrown;
}
.header__text {
  margin: auto;
  font-size: 15px;
  font-weight: bold;
}
.navbar {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  list-style: none;
  padding: 0;
  width: 100%;
  height: 72px;
  margin: 15px 0;
  padding: 0 30px
}
.nav__wrapper {
  display: flex;
  align-items: center;
}
.nav__wrapper__icon {
  width: 50px;
  height: 50px;
  cursor: pointer;
}
.navbar__logo {
  display: flex;
}
.navbar__logo__image {
  height: 72px;
  width: auto;
  margin: auto;
}
.navbar__actions {
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
.navbar__actions__icon {
  margin-left: 14px;
}
</style>
