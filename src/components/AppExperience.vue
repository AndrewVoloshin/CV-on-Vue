<template>
  <div class="experience">
    <div class="experience__bg-left"></div>
    <div class="experience__bg-right"></div>
    <div class="experience__container">
      <div class="experience__content">
        <h2>experience</h2>
        <p>What I am all about</p>
      </div>
      <p class="experience__text">experience__text</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style land="scss" scoped>
.experience {
  display: flex;
  justify-content: center;
  position: relative;
}
.experience__container {
  width: 100%;
}

.experience__content {
  padding: 1.5rem;
  background: #fafafa;
  border-top: solid 1px rgb(237, 237, 237);
  border-bottom: solid 1px rgb(237, 237, 237);
}

.experience__content h2 {
  margin-bottom: 7px;
}
.experience__text {
  padding: 1.5rem;
}

@media screen and (min-width: 600px) {
  .experience__text {
    font-size: 17px;
  }
}

@media screen and (min-width: 760px) {
  .experience__content {
    padding: 2.75rem 3.05rem;
  }
  .experience__text {
    padding: 2.75rem 3.05rem;
  }
  @media screen and (min-width: 1024px) {
    .experience__bg-left {
      top: 0;
      left: 0;
      position: absolute;
      height: 100%;
      width: 50%;
      background: #f8f8f8;
    }
    .experience__bg-right {
      top: 0;
      right: 0;
      position: absolute;
      height: 100%;
      width: 50%;
      background: #fcfcfc;
    }
    .experience__container {
      display: flex;
      position: relative;
      z-index: 2;
      max-width: 1276px;
    }
    .experience__content {
      width: 30%;
      border: none;
      text-align: right;
      background: #f8f8f8;
    }
    .experience__text {
      width: 70%;
      background: #fcfcfc;
    }
  }
  @media screen and (min-width: 1200px) {
    .experience__content {
      padding: 4.6rem;
    }
    .experience__text {
      padding: 4.6rem;
    }
  }
}
</style>
