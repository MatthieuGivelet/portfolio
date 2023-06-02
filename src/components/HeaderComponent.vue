<template>
    <main>
        <div class="txt-accueil">
            <div class="text-ligne">
                <!--<div class="shine"></div>-->
                <p class="ligne1">Bienvenue, <span class="deco"><a href="#about">Je suis Matthieu</a></span></p>
                <p class="ligne2">Graphiste & developpeur</p>
                <p class="ligne3">front end junior.</p>
                <div class ="feutre1"><img class ="img1" src="../assets/Rectangle 1.png" alt=""></div>
                <div class ="feutre2"><img class="img2" src="../assets/Rectancle 2.png" alt=""></div>
            </div>
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
    line-height: .1em;
    letter-spacing: -8.5px;
    margin-top: 2.3em;
    position: relative;
    z-index: 0;
}

/*.shine {
    position: absolute;
    z-index: 1;
    width: 400px;
    height: 300px;
    top: -50%;
    right: 50%;
    transform: skew(-40deg) translateX(-100px);
    background: linear-gradient(90deg, rgba(255, 255, 255, 0), rgba(255, 255, 255, 0.363));
    opacity: 0%;
    transition: .5s ease-in-out;
}

.text-ligne:hover .shine {
    opacity: 100%;
    transform: skew(-40deg) translateX(130px);
}

.text-ligne {
    transition: .5s ease-in-out;
}

.text-ligne:hover {
    transform: scale(110%);
}*/

.deco a {
    color:#4E4AFF;
    text-decoration: underline;
    transition: .3s ease-in-out;
}

.deco a:hover {
    color:#FFA53B;
}

/************ ANIM TEXT PRINCIPAL ************/

.ligne1 {
    animation-name: text;
    animation-duration: 1s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 0s;
}

.ligne2 {
    animation-name: text;
    animation-duration: 1s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: .2s;
}


.ligne3 {
    animation-name: text;
    animation-duration: 1s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: .4s;
}


@keyframes text {
    0% {
        transform: translateY(100px);
        filter: blur(10px);
        opacity: 0%;
    }

    40% {
        transform: translateY(-25px);
        filter: blur(0px);
        opacity: 100%;
    }

    100% {
        transform: translateY(0px);
        opacity: 100%;
    }
}

.feutre1, .feutre2 {
    z-index: -1;
    position: absolute;
}

.feutre1 {
    top: 52%;
    right: 55.5%;
    animation-name: animFeutre;
    animation-duration: .5s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 1s;
    
}

.feutre2 {
    top: 100%;
    right: 46%;
    animation-name: animFeutre;
    animation-duration: .5s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 1.2s;
}

/************ ANIM FEUTRE ************/

@keyframes animFeutre {
    from {
        transform: scaleX(0%);
        transform-origin: center left;
    }

    to {
        transform: scaleX(100%);
        transform-origin: center left;
    }
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

/************ ANIM TEXT SECONDAIRE ************/

.txt1 {
    animation-name: second;
    animation-duration: 1.5s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 1s;
}

.txt2 {
    animation-name: second;
    animation-duration: 1.5s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 1.2s;
}

@keyframes second {
    from {
        transform: translateY(50px);
        filter: blur(20px);
        opacity: 0%;
    }

    to {
        transform: translateY(0px);
        filter: blur(0px);
        opacity: 100%;
    }
}

</style>