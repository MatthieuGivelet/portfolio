<template>
  <header
    :class="currentScroll >= 100 ? 'active-navbar' : null"
  >
      <div class="nav">
        <RouterLink to ="/"><img src="../assets/Logo navbar.svg" alt=""></RouterLink>
          <div class="link">
          <a href="#about">A propos</a>
          <div class="lien-projet">
                 <RouterLink to = "/Projet">Projet </RouterLink>
                 <div class="chevron" @click="handleDropdownMenu">
                  <i class="fa-solid fa-chevron-down" @click="handlechevron" :class="rotate"></i>
                 </div>
                  
          </div>
        <div class="btn-nav">
          <a href="#contact">Contactez moi</a>
        </div>
        </div>
      </div>
      <MenuDeroulentComposent 
        v-if="showMenu"
        :class="animMenuOut"
      />
  </header>
</template>

<script>
import MenuDeroulentComposent from './MenuDeroulentComposent.vue'
  export default {
    data () {
      return {
        currentScroll: 0,
        showMenu: false,
        animMenuOut: null,
        rotate: null,
      }
    },
    components: {
      MenuDeroulentComposent
    },
    computed: {
      /* navBackground: function () {
        return this.currentScroll <= 100 ? "transparent" : "white"
      }, */
    },
    created () {
      window.addEventListener("scroll", this.handleScroll)
    },
    unmounted () {
      window.removeEventListener("scroll", this.handleScroll)
    },
    methods: {
      handleScroll: function () {
        this.currentScroll = window.scrollY
      },
      handleDropdownMenu() {
        if (this.showMenu) {
          this.animMenuOut = "anim-menu-out"
          setTimeout(
            () => {
              this.showMenu = false
            },
            400
          )
        } else {
          this.animMenuOut = null
          this.showMenu = true
        }
      },
      handlechevron() {
        if (this.showMenu) {
          this.rotate ="rotate"
        } else {
          this.rotate = "rotate-inverse"
        }
      }
    }
  }
</script>

<style scoped>

.rotate {
  transform: rotate(0deg);
}

.rotate-inverse {
  transform: rotate(180deg);
}


header {
  position: sticky;
  top: 0;
  z-index: 999;
  background-color: white;
  transition: .5s ease-in-out;
}

.nav, .link {
  display: flex;
  align-items: center;
  font-weight: 400;
}

.nav {
  max-width: 1280px;
  margin: auto;
  justify-content: space-between;
  padding: 2.5em;
}

.lien-projet {
  position: relative;
  display: flex;
}

.lien-projet i:hover {
  cursor: pointer;
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
  transition: .3s ease-in-out;
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

.active-navbar {
  background: rgb(255, 255, 255);
  box-shadow: 0px 5px 50px 0px rgba(50, 50, 93, 0.20);
}
</style>