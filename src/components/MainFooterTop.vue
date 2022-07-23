<template>
    <section id="main-footer-top">
        <div class="container">
            <nav>
                <div>
                    <h4>DC COMICS</h4>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h4>SHOP</h4>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div>
                    <h4>DC</h4>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div>
                    <h4>SITES</h4>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </nav>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MainFooterTop',
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/mixins';

#main-footer-top {
    @include bg-image('../assets/img/footer-bg.jpg');
    background-size: cover;


    nav {
        padding: 35px 0;
        @include bg-image('../assets/img/dc-logo-bg.png');
        background-position: right;
        display: flex;

        div {
            margin-right: 50px;
        }
    }

    h4,
    ul {
        margin-bottom: 15px;
    }

    h4 {
        color: #fff;
        font-size: 20px;
    }


    a {
        color: #A8A8A8;
        font-size: 12px;
    }
}
</style>