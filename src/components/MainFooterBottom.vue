<template>
    <section id="main-footer-bottom">
        <nav class="container">
            <a href="#" id="newsletter-sign-up">SIGN-UP NOW!</a>

            <div id="follow-us">
                <div>FOLLOW US</div>
                <div>
                    <a href=""><img src="../assets/img/footer-facebook.png" alt="Facebook Logo"></a>
                    <a href=""><img src="../assets/img/footer-twitter.png" alt="Twitter Logo"></a>
                    <a href=""><img src="../assets/img/footer-youtube.png" alt="Youtube Logo"></a>
                    <a href=""><img src="../assets/img/footer-pinterest.png" alt="Pinterest Logo"></a>
                    <a href=""><img src="../assets/img/footer-periscope.png" alt="Periscope Logo"></a>
                </div>
            </div>
        </nav>
    </section>
</template>

<script>
export default {
    name: 'MainFooterBottom',
}
</script>

<style scoped>
#main-footer-bottom {
    background-color: #303030;
}

#main-footer-bottom nav {
    padding: 30px 0;
    display: flex;
    justify-content: space-between;
}

#newsletter-sign-up {
    border: 2px solid #0282F9;
    padding: 10px 15px;
    color: #fff;
    font-size: 18px;
    font-weight: 500;
    transition: background-color 0.2s;
}

#newsletter-sign-up:hover {
    background-color: #0282F9;
    color: #000;
}

#follow-us {
    display: flex;
    align-items: center;
    font-size: 20px;
    color: #0282F9;
    font-weight: 700;
}

#follow-us div:first-of-type {
    margin-right: 15px;
}

#follow-us div:last-of-type {
    display: flex;
}

#follow-us a {
    margin: 0 10px;
}

#follow-us img {
    display: block;
    transition: transform 0.2s;
}

#follow-us a:hover img {
    transform: translateY(-5px);
}
</style>