<template>
    <div id="main-banner">
        <h1>Make your Burger</h1>
    </div>
</template>

<script>
export default {
    name: "Banner"
}
</script>

<style scoped>
    #main-banner{
        background-image: url('/public/img/burger.jpg');
        background-position: 0 -250px;
        background-size: cover;
        height: 500px;
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }

    #main-banner h1{
        color: #FFF;
        text-align: center;
        font-size: 60px;
        background-color: #222;
        padding: 20px 40px;
    }
</style>

<!-- background-size: cover; é para deixar a imagem aparecer no maximo da tela
display: flex; para posicionar melhor o h1 o texto
align-items: center; alinhar no centro o texto na horizontal
display: flex; para alinhar o texto na esquerda

padding: 20px 40px; para ter diferença de espaço nos cantos, assim aumentando o espaço e o fundo 
 -->