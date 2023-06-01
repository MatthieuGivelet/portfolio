<template>
  <main>
      <div class="nav">
    <RouterLink to ="/"><img src="../assets/Matthieu .G.png" alt=""></RouterLink>
    <div class="link">
          <a href="">A propos</a>
          <RouterLink to = "/Projet">Projet <i class="fa-solid fa-chevron-down"></i></RouterLink>
    <div class="btn-nav">
      <a href="">Contactez moi</a>
      <div class="anim"></div>
    </div>
    </div>
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

.nav, .link {
  display: flex;
  align-items: center;
  font-weight: 400;
}

.nav {
  justify-content: space-between;
  margin-top: 2.5em;
}

.link {
  gap: 3em;
}

.link a {
  color: #16161C;
  text-decoration: none;
}

.link i {
  margin-left: .5em;
}

.btn-nav a {
  color: white;
  padding: 1em 2em;
  background: #4E4AFF;
  border: 1px solid rgba(255, 255, 255, 0.103);
  border-radius: 30px;
  transition: .3s ease-in-out;
}

.btn-nav a:hover {
  background: #FFA53B;
}
</style>