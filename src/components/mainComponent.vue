<template>
    <main>
        <div class="container">
        <div id="left-ul">
        <ul>
            <li>DC COMICS</li>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
        </ul>
        <ul>
            <li>SHOP</li>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
        </ul>
        </div>
        <div id="center-ul">
        <ul>
            <li>DC </li>
            <li>Terms of Use</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
            <li>Pinco</li>
            <li>Pallo</li>
            <li>Never</li>
            <li>Give Up!!!</li>
        </ul>
        </div>
        <div id="right-ul">
            <ul>
            <li>Videos</li>
            <li>News</li>
            <li>Pinco</li>
            <li>Pallo</li>
            <li>Never</li>
            <li>Give Up!!!</li>
            </ul>
        </div>
    </div>
    </main>
</template>
  
<script>
export default {
    name: "mainComponent",
};
</script>
  
<style scoped lang="scss">
    main {
        background-image: url(../assets/img/footer-bg.jpg);
        height: 300px;
    }
  
.container {
    display: flex;
    justify-content: flex-start;
    gap: 30px;
    margin: 0 auto;
    max-width: 1000px;
}

#left-ul {
    padding-left: 30px;
}

ul {
    list-style: none;
    padding: 0;
    margin: 0;
    padding-top: 20px;
}
ul li {
    color: #ffffff;
}
ul li:first-child {
    font-size: 1.3em;
    padding-bottom: 5px;
}
</style>