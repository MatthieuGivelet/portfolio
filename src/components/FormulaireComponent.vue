<template>
<main id="contact">
    <div class="form">
        <img class="pastille" src="../assets/pastille.png" alt="">
        <p class="main-title">Votre projet </p>
        <div class="service">
            <div class="title1">
                <p>Services</p>
            </div>
            <input class="btn-input" v-model="prestation" type="radio" value="service1" id="service1">
            <label class="btn" :class="{active:prestation==='service1'}" for="service1">Graphisme</label>
            <input class="btn-input" v-model="prestation" type="radio" value="service2" id="service2">
            <label class="btn" :class="{active:prestation==='service2'}" for="service2">Web design</label>
            <input class="btn-input" v-model="prestation" type="radio" value="service3" id="service3">
            <label class="btn" :class="{active:prestation==='service3'}" for="service3">Integration</label>
            <input class="btn-input" v-model="prestation" type="radio" value="service4" id="service4">
            <label class="btn" :class="{active:prestation==='service4'}" for="service4">Motion design</label>
        </div>
        <div class="budget">
            <div class="title2">
                <p>Budget</p>
            </div>
            <input class="btn-input" v-model="budget" type="radio" value="budget1" id="budget1">
            <label class="btn" :class="{active:budget==='budget1'}" for="budget1">0 - 500</label>
            <input class="btn-input" v-model="budget" type="radio" value="budget2" id="budget2">
            <label class="btn" :class="{active:budget==='budget2'}" for="budget2">1000 - 3000</label>
            <input class="btn-input" v-model="budget" type="radio" value="budget3" id="budget3">
            <label class="btn" :class="{active:budget==='budget3'}" for="budget3">+ 10 000</label>
        </div>
        <div class="nom-prenom">
            <div class="nom">
                <p class="title-form">Nom</p>
                <input type="text" name="nom" v-model="nom">
            </div>
            <div class="prenom">
                <p class="title-form">Prenom</p>
                <input type="text" name="prenom" v-model="prenom">
            </div>
        </div>
        <div class="projet">
            <p class="title-form">Details du projet</p>
                <input type="text" name="details" v-model="details">
        </div>
        <div class="boutton-form">
            <button class="boutton">Envoyer</button>
        </div>
    </div>
</main>
</template>

<script>
export default {
    data () {
        return {
            prestation: null,
            budget: null
        }
    }
}
</script>

<style scoped>

main {
    max-width: 1280px;
    margin: auto;
    margin-bottom: 8em;
}

.service {
    margin-bottom: 4em;
}

.main-title {
    font-size: 3em;
    font-weight: 900;
    letter-spacing: -7px;
    margin: 0 0 1em 0;
}

.title1, .title2 {
    font-size: 1.2em;
    font-weight: 500;
    letter-spacing: -2px;
    padding-bottom: 1.5em;
}

.form {
    border: 1px solid rgba(0, 0, 0, 0.15);
    border-radius: 50px;
    padding: 4em 4em;
    position: relative;
}
.pastille {
    width: 120px;
    position: absolute;
    z-index: 1;
    top: -6%;
    right: 10%;
    filter: drop-shadow(0px 0px 0px #16161ce3);
    transition: .3s ease-in-out;
}

/*.pastille:hover {
    transform: scale(105%) rotate(10deg) translateY(-10px);
    filter: drop-shadow(0px 10px 3px #16161c48);
}*/

.btn-input {
    display: none;
}

.btn {
    font-size: small;
    background-color: #E6E6E6;
    border-radius: 30px;
    padding: 1.5em 3em;
    margin-right: 1em;
}

.btn.active {
    background-color: #4E4AFF;
    color: white;
}

.nom-prenom {
    margin-top: 4em;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nom, .prenom {
    display: inline-block;
}

*:focus {
    outline: none;
}

.title-form {
    font-size: 1.2em;
    font-weight: 500;
    letter-spacing: -2px;
    margin-bottom: 2em;
}

.nom input, .prenom input {
    width: 540px;
    border: none;
    border-bottom: 1px solid rgba(0, 0, 0, 0.15);
    margin-bottom: 2em;
}

.projet input {
    width: 100%;
    border: none;
    border-bottom: 1px solid rgba(0, 0, 0, 0.15);
}

.boutton {
    background-color: #4d4aff00;
    border: 1px solid rgba(0, 0, 0, 0.20);
    color: rgb(0, 0, 0);
    padding: 1em 2em;
    font-family: 'Lexend Exa', sans-serif;
    letter-spacing: -1px;
    border-radius: 30px;
    font-size: medium;
    margin-top: 4em;
    transition: .3s ease-in-out;
}

.boutton:hover {
    background-color: #4E4AFF;
    border: 1px solid rgba(255, 255, 255, 0.103);
    color: white;
}

</style>