<template>
  <HeaderComponent/>
  <div class="card-container">
    <CardComponent 
      :image="require('@/assets/1grauemeio.jpeg')"
      name="Um Grau e Meio"
    />

    <CardComponent 
      :image="require('@/assets/3AMining_institucional[10303].png')"
      name="3A Mining"
    />

    <CardComponent 
      :image="require('@/assets/brazil_foudation.png')"
      name="Brazil Foundation"
    />

    <CardComponent 
      :image="require('@/assets/institutoAcaia.jpeg')"
      name="Instituto Acaia"
    />

    <CardComponent 
      :image="require('@/assets/Logo_Inst.Localiza_principal.png')"
      name="Localiza"
    />

    <CardComponent 
      :image="require('@/assets/marca_sebrae_tagline_web.jpg')"
      name="Sebrae"
    />

    <CardComponent 
      :image="require('@/assets/ISA_CTEEP-logomarca-RGB[4928].png')"
      name="ISA CTEEP"
    />

    <CardComponent 
      :image="require('@/assets/Funbio-marca-vertical.svg.png')"
      name="Funbio"
    />

    <CardComponent 
      :image="require('@/assets/mupan.jpg')"
      name="Mupan Plano e Manejo"
    />

    <CardComponent 
      :image="require('@/assets/jef.png')"
      name="J&F Mineração"
    />

    <CardComponent 
      :image="require('@/assets/group.png')"
      name="Roberto Klabin"
    />

    <CardComponent 
      :image="require('@/assets/group.png')"
      name="Romeu Lacerda"
    />

    <CardComponent 
      :image="require('@/assets/group.png')"
      name="Teresa Bracher"
    />

    <CardComponent 
      :image="require('@/assets/group.png')"
      name="Reanto Teixeira"
    />

    <CardComponent 
      :image="require('@/assets/1grauemeio.jpeg')"
      name="Era"
    />

    <CardComponent 
      :image="require('@/assets/ISA_CTEEP-logomarca-RGB[4928].png')"
      name="ISA CTEEP / Conexão Jaguar"
    />

    <CardComponent 
      :image="require('@/assets/greatplans.png')"
      name="Great Plains Conservation"
    />

    <CardComponent 
      :image="require('@/assets/group.png')"
      name="A3 Arnoldo Valdi"
    />

    <CardComponent 
      :image="require('@/assets/greatplansfoundation.jpg')"
      name="Great Plains Foundation"
    />

    <!-- Inclua outros componentes CardComponent aqui -->
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue'
import CardComponent from './components/Card.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    CardComponent
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
}

.card-container {
  display: flex;
  justify-content: space-around; /* Espaçamento entre os cartões */
  flex-wrap: wrap; /* Permite que os cartões quebrem a linha se não houver espaço suficiente */
}
</style>
