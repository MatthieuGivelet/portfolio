<template>
    <div class="page">
        <i class="fa-solid fa-gear"></i>
        <div class="message">
            <p class="a1">En </p>
            <p class="a2">cours </p>
            <p class="a3">de </p>
            <p class="a4">fabrication</p>
        </div>
    </div>
</template>

<script>

</script>

<style>
.page {
    text-align: center;
    padding: 20em 20em;
}

.page i {
    font-size: 3em;
    color: rgba(0, 0, 0, 0.3);
    animation-name: roue;
    animation-duration: 10s;
    animation-iteration-count: infinite;
    animation-direction: initial;
    animation-timing-function: linear;
    animation-delay: 0s;
}

@keyframes roue {
    0% {
        transform: rotate(0deg);
    }

    100% {
        transform: rotate(360deg);
    }
}

.message {
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: .6em;
}

.message p {
    color: rgba(0, 0, 0, 0.3);
    font-size: 1.5em; 
    letter-spacing: -1px;
}

.a1 {
    animation-name: anim2;
    animation-duration: 10s;
    animation-iteration-count: infinite;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 0s;
}

.a2 {
    animation-name: anim2;
    animation-duration: 10s;
    animation-iteration-count: infinite;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 0.2s;
}

.a3 {
    animation-name: anim2;
    animation-duration: 10s;
    animation-iteration-count: infinite;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 0.4s;
}

.a4 {
    animation-name: anim2;
    animation-duration: 10s;
    animation-iteration-count: infinite;
    animation-direction: initial;
    animation-timing-function: ease-in-out;
    animation-fill-mode: backwards;
    animation-delay: 0.6s;
}



@keyframes anim2 {
    0% {
        transform: translateY(30px);
        filter: blur(10px);
        opacity: 0%;
    }

    10% {
        transform: translateY(0px);
        opacity: 100%;
        filter: blur(0px);
    }

    90% {
        transform: translateY(0px);
        opacity: 100%;
        filter: blur(0px);
    }

    100% {
        transform: translateY(-30px);
        filter: blur(10px);
        opacity: 0%;
    }
}

</style>

