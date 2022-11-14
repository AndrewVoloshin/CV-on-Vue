<template>
  <div class="brand">
    <h1>
      <span class="firstname">Andrew</span>
      <span class="lastname">Voloshin</span>
    </h1>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
h1 {
  text-align: center;
}

.firstname {
  display: block;
  font-weight: 300;
}
.lastname {
  display: block;
  color: #f8bb10;
  font-weight: 700;
  text-transform: uppercase;
}
@media screen and (min-width: 1024px) {
  .brand h1 {
    text-align: left;
  }
}

@media screen and (min-width: 1200px) {
  .brand h1 {
    font-size: 67px;
  }
}
</style>
