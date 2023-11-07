<template>
  <div class="brand">
    <h1>
      <span class="firstname start-move">Andrew</span>
      <span class="lastname start-move">Voloshin</span>
    </h1>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.start-move {
  opacity: 0;
  position: relative;
  bottom: -20px;
  transition: all 0.7s;
}
.move {
  opacity: 1;
  bottom: 0px;
}
.brand {
  font-size: 44px;
}

.brand h1 {
  font-size: 1em;
  line-height: 0.91;
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


</style>
