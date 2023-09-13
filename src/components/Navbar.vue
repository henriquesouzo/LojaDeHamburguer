<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/">Home</router-link> |
        <router-link to="/pedidos">Pedidos</router-link>
    </div>
</template>

<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
}
</script>

<style scoped>
    #nav{
        background-color: #222;
        border-bottom: 4px solid #111; 
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    #nav #logo-url{
        margin: auto;
        margin-left: 0;
    }

    #logo{
        width: 40px;
        height: 40px;
    }

    #nav a{
        color: #FCBA03;
        text-decoration: none;
        margin: 12px;
        transition: .5s;
    }

    #nav a:hover{
        color: #FFF;
    }
</style>
<!-- border-botton é para fazer uma borda em baixo 
padding é de 15px a altura limite de espaço e o 50 px é a horizontal para afastar
display é flex porque vai organizar um do lado do outro
justify-contente que é flex-end, vai começar da direita para a esquerda os itens do menu

na logo-url: margin auto para alinhar sozinho dependendo da tela
margin-left é a distancia de espaço da esquerda, como é 0 vai trazer bem ao lado esquerdo

nav a seria mudar os links das letras do menu, text-decoration: none porque tira o underline dos items
margin 12px é o afastamento entre os items
transition é o tempo de duração do efeito, quando passa o mouse por cima vai mudar de cor depois

nav a:hover é o tipo de ação quando passa o mouse em cima, vai ficar branco a cor das letras
-->
