<template>
    <div class="Carre"><img :src="imageUrl" alt=""></div>
</template>

<script>
export default {
    props: {
        image: String,
    },
    computed: {
        imageUrl: function () {
            return new URL(this.image, import.meta.url).href
        }
    }
}
</script>

<style scoped>
.Carre {
    background-color: #E6E4E4;
    border: 1px solid #cfcfcf;
    width: 30em;
    height: 25em;
    transition: .3s ease-in-out;
}

.Carre:hover {
    transform: scale(115%);
    box-shadow: 0px 10px 50px 5px rgba(0,0,0,0.2);
}

</style>