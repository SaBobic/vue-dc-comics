<template>
    <section id="main-footer-bottom">
        <nav class="container">
            <a href="#" class="newsletter-sign-up">SIGN-UP NOW!</a>

            <div class="follow-us c-primary">
                <div>FOLLOW US</div>
                <div>
                    <a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook Logo"></a>
                    <a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter Logo"></a>
                    <a href="#"><img src="../assets/img/footer-youtube.png" alt="Youtube Logo"></a>
                    <a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest Logo"></a>
                    <a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope Logo"></a>
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

<style lang="scss" scoped>
@import '../assets/sass/vars';

#main-footer-bottom {
    background-color: #303030;

    nav {
        padding: 30px 0;
        display: flex;
        justify-content: space-between;
    }

    .newsletter-sign-up {
        border: 2px solid $primary_color;
        padding: 10px 15px;
        color: #fff;
        font-size: 18px;
        font-weight: 500;
        transition: background-color 0.2s;

        &:hover {
            background-color: $primary_color;
            color: #000;
        }
    }

    .follow-us {
        display: flex;
        align-items: center;
        font-size: 20px;
        font-weight: 700;

        div {
            &:first-of-type {
                margin-right: 15px;
            }

            &:last-of-type {
                display: flex;
            }

            img {
                display: block;
                transition: transform 0.2s;
            }

            a {
                margin: 0 10px;

                &:hover img {
                    transform: translateY(-5px);
                }

            }
        }
    }
}
</style>