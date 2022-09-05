<template>
    <div class="shop__dc">
        <div class="container">
            <ul>
                <li>
                    <a href="">
                        <img src="../assets/buy-comics-digital-comics.png" alt="buy-comics-digital-comics">
                        <p>digital comics</p>
                    </a>
                </li>

                <li>
                    <a href="">
                        <img src="../assets/buy-comics-merchandise.png" alt="assets/buy-comics-merchandise">
                        <p>dc merchandise</p>
                    </a>
                </li>

                <li>
                    <a href="">
                        <img src="../assets/buy-comics-subscriptions.png" alt="buy-comics-subscriptions">
                        <p>subscription</p>
                    </a>
                </li>

                <li>
                    <a href="">
                        <img src="../assets/buy-comics-shop-locator.png" alt="buy-comics-shop-locator">
                        <p>comic shop locator</p>
                    </a>
                </li>

                <li>
                    <a href="">
                        <img src="../assets/buy-dc-power-visa.svg" alt="buy-dc-power-visa">
                        <p>dc power visa</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/variables';

.shop__dc {
    background-color: $blue-dc;

    .container {

        color: white;
        height: 155px;
        font-size: 1rem;
        display: flex;

        align-items: center;

        ul {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-basis: 100%;
            text-transform: uppercase;
            font-size: 12px;
            flex-wrap: wrap;
    

            li {
                flex-basis: calc(100% / 5);
            }

            a {
                display: flex;
                justify-content: center;
                align-items: center;
                gap: 18px;

                img {
                    max-height: 55px;
                    max-width: 55px;
                }

            }
        }
    }
}
</style>
