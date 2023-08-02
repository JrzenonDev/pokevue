<template>
  <div class="container mt-4 text-body-secondary">
    <div class="card">
      <h1 class="text-center">PokeVue</h1>
      <hr />
      <div class="card-body">
        <h2>Objetivo</h2>
        <p>
          Este é um projeto para fins didáticos utilizando Vue.js 3 com Vite.
        </p>
        <p>
          Link do projeto no Github:
          <a href="https://github.com/JrzenonDev/pokevue" target="_blank"
            >https://github.com/JrzenonDev/pokevue</a
          >
        </p>
        <hr />
        <h2>Recursos utilizados</h2>
        <p>
          Neste projeto, foram empregados recursos avançados como a
          <strong>Composition API</strong>.Além disso, foi realizada a
          utilização da <strong>Fetch API</strong> para efetuar requisições
          assíncronas à API de pokemons, buscando e exibindo dados em tempo
          real.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
@media (min-width: 1024px) {
  .container {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
</style>
