<template>
    <footer>
        <div><button>SIGN-UP NOW!</button></div>
        <div id="social">
            <div>FOLLOW US</div>
            <div>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
            </div>
        </div>
    </footer>
</template>
 
<script>
export default {
    name: "footerComponent",
};
</script>
  
<style scoped lang="scss">
footer {
    background-color: #303030;
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
footer div button {
    height: 50px;
    padding: 5px;
   color: #ffffff;
   border: 3px solid #0282f4;
   margin-left: 20px;
}
#social {
    display: flex;
    align-items: center;
    
}
#social div {
    color: #0282f4;
    padding-right: 20px;
}
</style>