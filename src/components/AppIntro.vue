<template>
  <div class="intro">
    <div class="intro__bg-left"></div>
    <div class="intro__bg-right"></div>
    <div class="intro__container">
      <div class="intro__content">
        <h2>intro</h2>
        <p>What I am all about</p>
      </div>
      <p class="intro__text">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Minima omnis
        laudantium perferendis ut autem commodi voluptatum id sed dignissimos
        ipsum consectetur doloremque nihil distinctio in, corporis hic totam,
        sint quo ullam. Quaerat obcaecati velit, temporibus reprehenderit,
        veritatis rem, labore totam laudantium explicabo ratione hic minus aut
        nobis animi at excepturi impedit error iure ipsa sint cumque porro.
        Sint, obcaecati ad, adipisci facere ducimus cupiditate quas suscipit
        labore eligendi soluta repudiandae doloremque accusamus autem aliquid
        velit eaque eum? Quas delectus natus consequuntur, nulla error sequi
        unde ipsum explicabo dolores alias cumque suscipit tempore, maiores
        iure, quam nemo tenetur obcaecati deserunt asperiores?
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style land="scss" scoped>
.intro {
  display: flex;
  justify-content: center;
  position: relative;
}
.intro__container {
  width: 100%;
}

.intro__content {
  padding: 1.5rem;
  background: #fafafa;
  border-top: solid 1px rgb(237, 237, 237);
  border-bottom: solid 1px rgb(237, 237, 237);
}

.intro__content h2 {
  margin-bottom: 7px;
}
.intro__text {
  padding: 1.5rem;
}

@media screen and (min-width: 600px) {
  .intro__text {
    font-size: 17px;
  }
}

@media screen and (min-width: 760px) {
  .intro__content {
    padding: 2.75rem 3.05rem;
  }
  .intro__text {
    padding: 2.75rem 3.05rem;
  }
  @media screen and (min-width: 1024px) {
    .intro__bg-left {
      top: 0;
      left: 0;
      position: absolute;
      height: 100%;
      width: 50%;
      background: #f8f8f8;
    }
    .intro__bg-right {
      top: 0;
      right: 0;
      position: absolute;
      height: 100%;
      width: 50%;
      background: #fcfcfc;
    }
    .intro__container {
      display: flex;
      position: relative;
      z-index: 2;
      max-width: 1276px;
    }
    .intro__content {
      width: 30%;
      border: none;
      text-align: right;
      background: #f8f8f8;
    }
    .intro__text {
      width: 70%;
      background: #fcfcfc;
    }
  }
  @media screen and (min-width: 1200px) {
    .intro__content {
      padding: 4.6rem;
    }
    .intro__text {
      padding: 4.6rem;
    }
  }
}
</style>
