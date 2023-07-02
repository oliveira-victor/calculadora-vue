<script setup>
const bgColor = () => {
    //document.querySelector('body').style.background = '#494949'
    document.querySelector('body').style.backgroundImage = 'url(https://www.svgbackgrounds.com/wp-content/uploads/2021/05/square-versatiles-yellow-subtle-pattern.jpg)'
}
bgColor()
</script>

<template>
<div class="container">
    <header>
        <h1>Calculadora</h1>
    </header>
    <div class="main">
        <form>
            <input required type="number" placeholder="0">
            <input required type="number" placeholder="0">
            <select class="select">
                <option value="adicao">Adição +</option>
                <option value="subtração">Subtração -</option>
                <option value="multiplicacao">Multiplicação *</option>
                <option value="divisao">Divisão /</option>
            </select>
        </form>
        <div class="results">
            O resultado da conta é:<br />
            <div class="number">
                0
            </div>
        </div>
    </div>
</div>
    <footer>
        Site desenvolvido por Victor F. Oliveira<br />
        <a href="https://github.com/oliveira-victor" target="_blank">github.com/oliveira-victor</a>
    </footer>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Ubuntu', sans-serif;
    font-size: 24px;
}
.container {
    width: 800px;
    margin: 10% auto;
    text-align: center;
    box-shadow: 0px 10px 15px rgba(0, 0, 0, 0.7);
    border-radius: 40px;
}
header {
    background-color: #222222;
    color: #dbbf60;
    padding: 16px;
    border-radius: 40px 40px 0 0;
}
.main {
    background-color: #dbbf60;
    border-radius: 0 0 40px 40px;
}
form {
    padding-top: 40px;
}
input  {
    width: 120px;
    height: 40px;
    padding: 6px;
    margin: 6px;
    border-radius: 8px;
}
.select {
    width: 140px;
    height: 40px;
    margin: 6px;
    border-radius: 8px;
}
.results {
    margin-top: 40px;
}
.number {
    font-size: 46px;
    font-weight: bold;
    margin-top: 10px;
    padding-bottom: 40px;
}
footer {
    width: 70%;
    margin: 0 auto;
    text-align: center;
    font-size: 18px;
}
footer a {
    font-size: 18px;
    text-decoration: none;
    color: #a11919;
}
footer a:hover {
    text-decoration: underline;
}
</style>
