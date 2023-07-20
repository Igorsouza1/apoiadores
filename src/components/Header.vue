<template>
  <header class="header">
    <div class="title">APOIADORES IHP</div>
    <nav id="menu">
      <ul>
        <li><a href="#" @click="setActive('REDE')" :class="{ active: activeItem === 'REDE' }">REDE</a></li>
        <li><a href="#" @click="setActive('FELINOS')" :class="{ active: activeItem === 'FELINOS' }">FELINOS</a></li>
        <li><a href="#" @click="setActive('CABECEIRAS')" :class="{ active: activeItem === 'CABECEIRAS' }">CABECEIRAS</a></li>
        <li><a href="#" @click="setActive('BRIGADA')" :class="{ active: activeItem === 'BRIGADA' }">BRIGADA</a></li>
        <li><a href="#" @click="setActive('AMOLAR_EXPERIENCE')" :class="{ active: activeItem === 'AMOLAR_EXPERIENCE' }">AMOLAR EXPERIENCE</a></li>
        <li><a href="#" @click="setActive('MEMORIAL')" :class="{ active: activeItem === 'MEMORIAL' }">MEMORIAL</a></li>
        <li><a href="#" @click="setActive('BARCOS')" :class="{ active: activeItem === 'BARCOS' }">BARCOS</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      activeItem: 'REDE', // O item ativo inicial é 'REDE'
    }
  },
  methods: {
    setActive(item) {
      this.activeItem = item; // Quando um item do menu é clicado, ele se torna o item ativo
    },
  },
}
</script>

<style scoped>
.header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #103d33;
  padding: 2em;
}

.title {
  font-size: 1.5em;
  font-weight: bold;
  color: white;
  margin-bottom: 0.3em; /* Espaço entre o título e o menu */
}

#menu ul {
  list-style: none;
  display: flex;
  flex-wrap: wrap; /* Permite que os itens do menu quebrem a linha */
  justify-content: center; /* Centraliza os itens do menu quando eles quebram a linha */
  gap: 0.8em;
  margin-top: 10px;
}

#menu ul li{
  padding: 0.8em;
}

#menu ul li a {
  text-decoration: none;
  color: #ffffff;
  padding: 0.5em 1em;
  border-radius: 0.3em;
  border: 0.1em solid rgb(255, 255, 255);
  transition: all 0.3s ease;
}

#menu ul li a.active {
  background-color: white;
  color: black;
  box-shadow: rgba(50, 50, 93, 0.1) 0px 30px 60px -12px inset, rgba(0, 0, 0, 0.2) 0px 18px 36px -18px inset;
}
</style>
