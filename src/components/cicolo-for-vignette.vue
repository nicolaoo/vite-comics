

<script>
export default {
    props: {
        src: String,
        text: String,

    }
}

</script>


<template>
    <div class="card">
        <figure>
            <img :src="src" alt="">
        </figure>
        <p>
            {{ text }}
        </p>
    </div>
</template>

<style lang="scss" scoped>
.card {
    p {
        color: white;
        text-transform: uppercase;
        font-size: 10px;
    }
}
</style>