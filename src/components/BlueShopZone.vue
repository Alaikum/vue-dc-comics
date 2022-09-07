<template>
    <div class="shop__dc">
        <div class="container">
            <ul>
                <li v-for="(el,id) in shopBlue" :key="id">
                    <a href="#">
                        <img :src="el.img" alt="buy-comics-digital-comics">
                        <p>{{el.text}}</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            shopBlue: [
                {
                    img: require("../assets/buy-comics-digital-comics.png"),
                    text: 'Digital Comics'
                },
                {
                    img: require("../assets/buy-comics-merchandise.png"),
                    text: 'Dc Merchandise'
                },
                {
                    img: require("../assets/buy-comics-subscriptions.png"),
                    text: 'Subscription'
                },
                {
                    img: require("../assets/buy-comics-shop-locator.png"),
                    text: 'Comic Shop Locator'
                },
                {
                    img: require("../assets/buy-dc-power-visa.svg"),
                    text: 'Dc Power Visa'
                }
            ]
        }
    }

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
