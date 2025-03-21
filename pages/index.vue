<!-- src/App.vue -->
<template>
  <div id="app">
    <!-- Usamos los componentes Header, Card y Footer -->
    <Header />
    <Card title="Componente de Tarjeta 1" description="Este es el primer componente de tarjeta." />
    <Card title="Componente de Tarjeta 2" description="Este es el segundo componente de tarjeta." />
    <Footer />
  </div>
</template>

<script>
// Importamos los componentes
import Card from '/components/Card.vue';
import Footer from '/components/Footer.vue';
import Header from '/components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
    Card,
    Footer
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin: 20px;
}
</style>
