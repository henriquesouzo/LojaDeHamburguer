<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <router-view/>
  <Footer />
</template>

<script>
  import Navbar from "./components/Navbar.vue"
  import Footer from "./components/Footer.vue"

export default {
  components: {
    Navbar,
    Footer
  },
  data(){
    return{
      logo_src: "img/logo.png",
      app_name: "Make your Burger"
    }
  }
}
</script>

<style>
  * {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-container{
    margin: 50px;
    min-height: 250px;
  }

  h1{
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>

<!-- Vou dizer que todos os elementos vai ter a font Helvetica
vou tirar todos os padding e margin que assim vai preencher todos os cantos da tela e alinhar melhor e tirar os espaçamentos
box-sizing border-box serve para todos os input não passar da div vai

como a classe main-container esta em mais de um lugar como em Home e em Pedidos, eu posso alterar os dois em um lugar só
mesma coisa estou alterando todos <h1> de uma vez
margin-bottom serve para afastar o conteudo que fica abaixo dele, dar um espaço

-->
