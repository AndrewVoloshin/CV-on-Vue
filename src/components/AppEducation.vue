<template>
  <div class="education">
    <div class="education__bg-left"></div>
    <div class="education__bg-right"></div>
    <div class="education__container">
      <div class="education__title">
        <h2>education</h2>
        <p>What I am all about</p>
      </div>
      <div class="education__content">
        <div class="education__timeline">
          <app-timeline
            :item="item"
            v-for="item in education"
            :key="item"
          ></app-timeline>
          <div class="content__end"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { education } from "@/assets/experience.js";
import AppTimeline from "./AppTimeline.vue";

export default {
  components: { AppTimeline },
  data() {
    return {
      education: education,
    };
  },
};
</script>

<style land="scss" scoped>
.education {
  display: flex;
  justify-content: center;
  position: relative;
}
.education__container {
  width: 100%;
}

.education__title {
  padding: 1.5rem;
  background: #fafafa;
  border-top: solid 1px rgb(237, 237, 237);
  border-bottom: solid 1px rgb(237, 237, 237);
}

.education__title h2 {
  margin-bottom: 7px;
}
.education__content {
  padding: 1.5rem 0 0 1.5rem;
}
.education__timeline {
  position: relative;
}
.content__end {
  position: absolute;
  left: 5px;
  bottom: 0;
  width: 16px;
  height: 2px;
  background: #ececec;
}

.item__title {
}

.education__text {
}

@media screen and (min-width: 600px) {
  .education__content {
    /* font-size: 17px; */
  }
}

@media screen and (min-width: 760px) {
  .education__title {
    padding: 2.75rem 3.05rem;
  }
  .education__content {
    padding: 2.75rem 3.05rem;
  }
}

@media screen and (min-width: 1024px) {
  .education__bg-left {
    top: 0;
    left: 0;
    position: absolute;
    height: 100%;
    width: 50%;
    background: #f8f8f8;
  }
  .education__bg-right {
    top: 0;
    right: 0;
    position: absolute;
    height: 100%;
    width: 50%;
    background: #fcfcfc;
  }
  .education__container {
    display: flex;
    position: relative;
    z-index: 2;
    max-width: 1276px;
  }
  .education__title {
    width: 30%;
    border: none;
    text-align: right;
    background: #f8f8f8;
  }
  .education__content {
    width: 70%;
    background: #fcfcfc;
  }
}
@media screen and (min-width: 1200px) {
  .education__title {
    padding: 4.6rem;
  }
  .education__content {
    padding: 4.6rem;
  }
}
</style>
