<template>
  <header>
    <NavBar />
  </header>
  <main>
    <Content />
  </main>
</template>

<script>
import NavBar from './components/NavBar.vue'
import Content from './components/Content.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Content
  },
  created() {
    const cardItems = [
      {
        imagen: "https://cdn.shopify.com/s/files/1/0595/9915/9452/products/13685459_59FIFTY_LMB_AWAY_LEOBRA_GRN_3QL_2048x.png",
        descripcion: "Bravos de León LMB Game Cap Away 59FIFTY Cerrada Verde",
        precio: 999.00
      },
      {
        imagen: "https://cdn.shopify.com/s/files/1/0595/9915/9452/products/60354481_59FIFTY_CITYCONNECTSEAMAR_SEAMAR_OTC_3QL_750x750.png",
        descripcion: "Seattle Mariners MLB City Connect 59FIFTY Cerrada",
        precio: 999.00
      },
      {
        imagen: "https://cdn.shopify.com/s/files/1/0595/9915/9452/products/60355750_59FIFTY_MLB23MTHRSDAY_NEYYAN_STN_3QR_750x750.png",
        descripcion: "New York Yankees MLB Mother's Day 2023 59FIFTY Cerrada",
        precio: 999.00
      },
      {
        imagen: "https://cdn.shopify.com/s/files/1/0595/9915/9452/products/13740148_59FIFTY_MLB_MX_GAME_BLK_3QR_c8ba2c98-904b-4f52-8398-a141b824858a_750x750.png",
        descripcion: "MLB Logo Mexico City Series 2023 59FIFTY Cerrada",
        precio: 999.00
      },
      {
        imagen: "https://cdn.shopify.com/s/files/1/0595/9915/9452/products/13574796_59FIFTY_LMB_BASIC_MEXDIA_BL_3QL_750x750.png",
        descripcion: "Diablos Rojos del México LMB Game Cap Alternativa Menta 59FIFTY Cerrada",
        precio: 999.00
      },
      {
        imagen: "https://cdn.shopify.com/s/files/1/0595/9915/9452/products/13701470_59FIFTY_WBC_MEXMEX_KELLY_GRN_3QR_750x750.png",
        descripcion: "México Game Cap Home MLB World Baseball Classic 2023 59FIFTY Cerrada",
        precio: 999.00
      }
    ]

    localStorage.setItem('cardItems', JSON.stringify(cardItems))
  }
}
</script>

<style>

</style>
