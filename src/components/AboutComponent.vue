<template>
    <div class="cadre">
            <div class="block">
            <section class="about">
        <div class="txt">
            <div class="title3">
                <p>Lorem ipsum dolor sit amet,<br>consectetur adipiscing.</p>
            </div>
            <div class="feutre3">
                <img src="../assets/Rectangle violet.png" alt="">
            </div>
            <div class="texte">
                <p>Sed do eiusmod tempor incididunt ut labore et dolore magna<br>aliqua. Ut enim ad minim veniam, quis nostrud exercitation<br>ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis<br>aute irure dolor in reprehenderit in voluptate velit esse cillum<br>dolore eu fugiat nulla pariatur.</p>
            </div>
            <div class="boutton">
                <a class="btn2" href="">Curriculum</a>
                <a class="btn3" href=""><i class="fa-solid fa-download"></i></a>
            </div>
        </div>
        <div class="photo">
            <img src="../assets/Portait.jpg" alt="">
        </div>
        <div class="stars">
            <img src="../assets/Stars.png" alt="">
        </div>
    </section>
    </div>
    <div class="counter">
        <div class="left">
            <p>Projets<br>réalisés</p>
        </div>
        <div class="rignt">
            <div class="count1">
                <p class="titre">Graphique<br>design</p>
                <p class="number">07</p>
            </div>
            <div class="count2">
                <p class="titre">Web<br>design</p>
                <p class="number">02</p>
            </div>
            <div class="count3">
                <p class="titre">Motion<br>design</p>
                <p class="number">04</p>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
export default {}
</script>

<style>


/************* ABOUT *************/

.block {
    background: #16161C;
    color: white;
    padding: 11em 20em 20em 20em;
    position: relative;
    z-index: -3;
    overflow: hidden;
    margin-bottom: 15em;
}

.photo img {
    position: absolute;
    z-index: -2;
    top: 0;
    right: -5%;
    width: 75%;
    mix-blend-mode: lighten;
    filter: grayscale(100%);
}

.title3 {
    font-size: 3em;
    line-height: 1em;
    letter-spacing: -5px;
    font-weight: 700;
}

.feutre3 {
    position: absolute;
    z-index: -1;
    top: 33%;
    right: 50.5%;
}

.stars {
    position: absolute;
    z-index: -1;
    top: 45%;
    right: 42%;
}

.texte {
    color: #8786A9;
    margin-bottom: 5em;
}

.btn2 {
    text-decoration: none;
    color: white;
    padding: 1em 2em;
    background: #4E4AFF;
    border-radius: 30px;
    border: 1px solid rgba(255, 255, 255, 0.103);
}

.btn3 {
    padding: 1em 1em;
    background: #4d4aff4b;
    border-radius: 50px;
    margin-left: 1em;
    border: 1px solid rgba(255, 255, 255, 0.027);
}

.btn3 i {
    color: white;
    font-size: 1.3em;
}

/************* COUNTER *************/

.cadre {
    position: relative;
}

.counter {
    position: absolute;
    z-index: 1;
    top: 88%;
    left: 22.3%;
    /*max-width: 1000px;*/
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #4E4AFF;
    color: white;
    border-radius: 20px;
    border: 1px solid rgba(255, 255, 255, 0.103);
    box-shadow: 0px 10px 50px 5px rgba(0,0,0,0.2);
    overflow: hidden;
}

.left p {
    font-size: 1.5em;
    font-weight: 700;
    line-height: 1em;
    letter-spacing: -2px;
}

.left {
    background: #00000015;
    padding: 3.5em 5em;
}

.rignt {
    display: flex;
    align-items: center;
    gap: 3em;
}

.count1, .count2, .count3 {
    display: flex;
    align-items: center;
    font-weight: 700;
    color: rgba(255, 255, 255, 0.5);
    gap: 1em;
    height: 3em;
}

.count1, .count2 {
    border-right: 1px solid white;
    padding: 0 2.5em 0 0;
}

.count1 {
    padding: 0 2.5em 0 4em;
}

.count3 {
    padding: 0 5em 0 0;
}

.number {
    font-size: 3em;
    color: white;
}

.titre {
    font-weight: 500;
}


</style>