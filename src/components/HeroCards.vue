<template>

    <div class="card">
        <figure>
            <img :src="thumb" alt="">
        </figure>
        <p>{{ series }}</p>
    </div>



</template>

<script>
export default {
    props: {
        thumb: String,
        series: String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card {
    display: flex;
    flex-direction: column;
    align-items: center;

    figure {
        max-height: 185px;
        overflow: hidden;

    }

    p {
        padding: 20px 0;
        font-weight: 700;
    }
}
</style>
