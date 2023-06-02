<template>
<div class="menu">
    <router-link to="/projet">Graphique design</router-link>
    <router-link to="/projet">Web design</router-link>
    <router-link to="/projet">Illustration</router-link>
    <router-link to="/projet">Integration</router-link>
    <router-link to="/projet">Animation</router-link>
</div>
</template>

<script>
export default {}
</script>

<style>
.menu {
    position: absolute;
    display: flex;
    gap: 1em;
    flex-direction: column;
    width: max-content;
    background-color: rgb(255, 255, 255);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255, 255, 255, 0.192);
    padding: 2.5em 8em 2.5em 3em;
    border-radius: 20px;
    right: 18%;
    box-shadow: 0px 10px 80px 5px rgba(0,0,0,0.20);
    animation-name: anim-in;
    animation-duration: .4s;
    animation-iteration-count: initial;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 0s;
}

.anim-menu-out {
  animation-name: anim-out;
  animation-duration: .45s;
  animation-iteration-count: initial;
  animation-direction: initial;
  animation-timing-function: ease-in-out;
  animation-fill-mode: backwards;
  animation-delay: 0s;
}

@keyframes anim-in {
    from {
        transform: translateY(-20%);
        opacity: 0%;
    }

    to {
        transform: translateY(0%);
        opacity: 100%;
    }
}

@keyframes anim-out {
    from {
        transform: translateY(0%);
        opacity: 100%;
    }

    to {
        transform: translateY(-20%);
        opacity: 0%;
    }
}

.menu a {
    text-decoration: none;
    color: black;
    transition: .2s ease-in-out;
}

.menu a:hover {
    color: #4E4AFF;
    transform: scale(110%) translateX(5%);
}
</style>