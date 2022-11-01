<template>
  <div class="experience">
    <div class="experience__bg-left"></div>
    <div class="experience__bg-right"></div>
    <div class="experience__container">
      <div class="experience__title">
        <h2>experience</h2>
        <p>What I am all about</p>
      </div>
      <div class="experience__content">
        <div class="experience__item">
          <div class="point"></div>
          <div class="item__title">
            <p>2015 – Present</p>
            <h3>Vichit</h3>
            <h4>Front-end Developer</h4>
          </div>
          <div class="experience__text">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus
              voluptates est deleniti animi labore dolorum quisquam repellat
              nam, aliquam sunt. Sequi, laboriosam vitae! Officia labore eius
              nostrum maiores aut amet esse soluta vero doloribus autem incidunt
              culpa, itaque mollitia aspernatur!
            </p>
          </div>
        </div>
        <div class="experience__item">
          <div class="point"></div>
          <div class="item__title">
            <p>2015 – Present</p>
            <h3>Vichit</h3>
            <h4>Front-end Developer</h4>
          </div>
          <div class="experience__text">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus
              voluptates est deleniti animi labore dolorum quisquam repellat
              nam, aliquam sunt. Sequi, laboriosam vitae! Officia labore eius
              nostrum maiores aut amet esse soluta vero doloribus autem incidunt
              culpa, itaque mollitia aspernatur!
            </p>
          </div>
        </div>
      </div>
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

.experience__title {
  padding: 1.5rem;
  background: #fafafa;
  border-top: solid 1px rgb(237, 237, 237);
  border-bottom: solid 1px rgb(237, 237, 237);
}

.experience__title h2 {
  margin-bottom: 7px;
}
.experience__content {
  padding: 1.5rem 0 0 1.5rem;
}

.experience__item {
  position: relative;
  padding: 0 0 0 1.5rem;
  border-left: 2px solid #ececec;
  margin-left: 12px;
  padding-bottom: 2rem;
}
.point {
  position: absolute;
  top: 0;
  left: -6px;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #f8bb10;
  /* margin-left: -6px; */
  box-shadow: 0 0 0 6px white;
}
.item__title {
}
.item__title p {
  opacity: 0.6;
  font-size: 10px;
  margin-bottom: 0.35rem;
}
.item__title h3 {
  color: #727272;
  text-transform: uppercase;
  font-size: 17px;
  line-height: 1.45;
  margin-bottom: 0.35rem;
}
.item__title h4 {
  font-size: 11px;
  font-weight: 500;
  margin-bottom: 0.35rem;
  color: #727272;
}
.experience__text {
}

@media screen and (min-width: 600px) {
  .experience__content {
    /* font-size: 17px; */
  }
}

@media screen and (min-width: 760px) {
  .experience__title {
    padding: 2.75rem 3.05rem;
  }
  .experience__content {
    padding: 2.75rem 3.05rem;
  }
  .experience__item{
    display: flex;
  }
  .item__title{
    width: 42%;
  }
  .experience__text{
    width: 58%;
  }
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
    .experience__title {
      width: 30%;
      border: none;
      text-align: right;
      background: #f8f8f8;
    }
    .experience__content {
      width: 70%;
      background: #fcfcfc;
    }
  }
  @media screen and (min-width: 1200px) {
    .experience__title {
      padding: 4.6rem;
    }
    .experience__content {
      padding: 4.6rem;
    }
  }

</style>
