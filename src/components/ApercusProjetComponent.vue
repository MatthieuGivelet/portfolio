<template>
    <main>
        <div class="title">
            <p>Projets récent</p>
            <a href="">Voir plus</a>
        </div>
        <div class="apercus">
            <CardComponent image=""/>
            <CardComponent />
            <CardComponent />
            <CardComponent />
        </div>
    </main>
</template>

<script>
    import CardComponent from './CardComponent.vue';
    export default {
        components: {
            CardComponent
        }
    }
</script>

<style>

main {
    margin-top: 8em;
}

.title {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1280px;
    margin: auto;
}

.title a {
    color: #16161C;
    font-weight: 500;
}

.apercus {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 2em;
}



</style>