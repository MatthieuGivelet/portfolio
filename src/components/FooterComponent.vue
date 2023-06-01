<template>
<div class="footer">
    <div class="container-footer">
        <div class="left-footer">
            <div class="txt-footer">
                <img src="../assets/Logo Footer.png" alt="">
                <p>Graphiste & developpeur front end junior.</p>
            </div>
            <div class="social">
                    <i class="fa-brands fa-dribbble"></i>
                    <i class="fa-brands fa-linkedin-in"></i>
            </div>
        </div>
        <div class="right-footer">
            <div class="list1">
                <a href="">Graphique design</a>
                <a href="">Web design</a>
                <a href="">Illustration</a>
                <a href="">Integration</a>
                <a href="">Animation</a>
            </div>
            <div class="list2">
                <a href="">Contact</a>
                <a href="">A propos</a>
                <a href="">Conditions de services</a>
                <a href="">Politique de confidentialité</a>
                <a href="">Paramétres des cookies</a>
            </div>
        </div>
    </div>
    <div class="copy">
        <p class="copyright">© 2023 Copyright Matthieu Givelet.</p>
    </div>
</div>
</template>

<script>
export default {}
</script>

<style>

.footer {
    background: #16161C;
}

.container-footer {
    display: flex;
    justify-content: space-between;
    max-width: 1280px;
    margin: auto;
    padding: 4em 0 4em 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.20);
}

.left-footer {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: white;
    font-size: small;
}

.right-footer {
    display: flex;
    align-items: center;
    gap: 15em;
}

.list1 a, .list2 a {
    font-size: small;
    text-decoration: none;
    color: white;
}

.list1, .list2 {
    display: flex;
    flex-direction: column;
    gap: 1em;
}

.copy {
    font-size: .7em;
    font-weight: 300;
    color: rgba(255, 255, 255, 0.20);
    padding: 2em 0 2em 0;
    text-align: center;
}

.social {
    display: flex;
    gap: 1.5em;
}

.social i {
    color: white;
    font-size: 2em;
    transition: .2s ease-in-out;
}

.social i:hover {
    color: #FFA53B;
    transform: scale(120%);
}

</style>
