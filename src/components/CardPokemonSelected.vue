<script setup>
const pokemon = defineProps(["name", "xp", "height", "image", "loading"]);
</script>

<template>
  <div
    class="card card-pokemon-selected"
    :class="loading ? '' : 'animate__animated animate__flipInY'"
  >
    <img
      v-if="pokemon.name"
      :src="pokemon.image"
      class="card-img-top"
      :alt="pokemon.name"
      height="350"
    />
    <img
      v-else
      src="../assets/egg_pokemon.svg"
      class="card-img-top"
      alt="..."
      height="350"
    />
    <div class="card-body">
      <h5 class="card-title text-center">{{ pokemon.name || "???" }}</h5>
      <hr />
      <div class="row">
        <section class="col">
          <strong>XP:</strong>
          <span>{{ pokemon.xp }}</span>
        </section>
        <section class="col">
          <strong>Altura:</strong>
          <span>{{ pokemon.height }}</span>
        </section>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card-pokemon-selected {
  height: 75vh;
  background: rgb(251, 138, 63);
  background: radial-gradient(
    circle,
    rgb(128, 245, 129) 0%,
    rgba(205, 100, 203, 0.11) 100%
  );
  cursor: pointer;
}
</style>
