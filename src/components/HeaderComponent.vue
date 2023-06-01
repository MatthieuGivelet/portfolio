<template>
    <main>
        <div class="txt-accueil">
            <p>Bienvenue, <span>Je suis Matthieu</span><br/>Graphiste & developpeur<br/>front end junior.</p>
            <img class ="feutre1" src="../assets/Rectangle 1.png" alt="">
            <img class ="feutre2" src="../assets/Rectancle 2.png" alt="">
        </div>
        <div class="texte-2">
            <div class="txt1">Création d’identité visuel : <br>logo & illustration.<br/> <div class="separator"></div> </div>
            <div class="txt2">Comception de site vitrine : <br>Web design & integration.<br/> <div class="separator"></div> </div>
        </div>
    </main>
</template>

<script>
    export default {}
</script>

<style scoped>
main {
    max-width: 1280px;
    margin: auto;
}

p {
    color: #16161C;
}

.txt-accueil {
    text-align: center;
    font-weight: 900;
    font-size: 4em;
    line-height: 1em;
    letter-spacing: -8.5px;
    margin-top: 2.3em;
    position: relative;
}

span {
    color:#4E4AFF;
    text-decoration: underline;
}

.feutre1, .feutre2 {
    z-index: -1;
    position: absolute;
}

.feutre1 {
    top: 52%;
    right: 55.5%;
}

.feutre2 {
    top: 85%;
    right: 46%;
}

/*********** Partie 2 ***********/

.texte-2 {
    color: #16161C;
    margin-top: 10em;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 6em;
    font-weight: 700;
    letter-spacing: -1.5px;
}

.separator {
    margin-top: 1.5em;
    background-color: #16161C;
    width: 50px;
    height: 3px;
}

</style>