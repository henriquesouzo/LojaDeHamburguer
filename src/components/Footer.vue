<template>
    <footer id="footer">
        <p>Make your Burger &copy; 2022</p>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped>
#footer{
    height: 200px;
    background-color: #222;
    border-top: 4px solid #111;
    color: #FCBA03;
    display: flex;
    align-items: center;
    justify-content: center;
    bottom: 0;
    width: 100%;
}
</style>

<!-- height é a altura
background-color é a cor de fundo
border-top é uma borda que fica acima fazendo uma linha
color é a cor dos textos
display é flex porque vai organizar um do lado do outro
align-items: center porque vai centralizar o conteudo
justify-content: center vai centralizar na vertical e horizontal
bottom: 0 so para fixar ele no centro para garantir
width: 100% que ele vai preencher toda a area
position: absolute para fixar sempre no final da pagina independente da altura da tela
-->