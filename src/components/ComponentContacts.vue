<template>
  <div class="contacts">
    <div v-if="displayHr" class="header__hr"></div>
    <div :class="['header__contacts', { 'text__align-start': textAlignStart }]">
      <div :class="['contact__item', { 'text__align-start': textAlignStart }]">
        <h4>Location</h4>
        <address>Ukraine, Kharkiv</address>
      </div>
      <div :class="['contact__item', { 'text__align-start': textAlignStart }]">
        <h4>Phone</h4>
        <p>+38(099)111-51-91</p>
      </div>
      <div :class="['contact__item', { 'text__align-start': textAlignStart }]">
        <a
          href="#"
          :class="['contact__link', { 'text__align-start': textAlignStart }]"
        >
          <h4>Web</h4>
          <p>youtube.com</p>
        </a>
      </div>
      <div :class="['contact__item', { 'text__align-start': textAlignStart }]">
        <h4>Email</h4>
        <p>VoloshinAndy@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["displayHr", "textAlignStart"],
};
</script>

<style lang="scss" scoped>
.header__hr {
  width: 100%;
  height: 2px;
  background-color: rgb(237, 237, 237);
  margin-bottom: 24.5px;
}
.header__contacts {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.contact__item {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 24.5px;
}
.contact__item h4 {
  color: #727272;
  font-weight: 600;
  margin-bottom: 8px;
}
.contact__item address {
  font-weight: 400;
  font-style: normal;
}

.contact__link {
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: color 0.15s linear;
  &:hover {
    color: #f8bb10;
  }
}

.text__align-start {
  align-items: flex-start;
}

@media screen and (min-width: 600px) {
  .header__contacts {
    width: 100%;
    flex-direction: row;
    flex-wrap: wrap;
  }

  .contact__item {
    width: 50%;
  }
}
@media screen and (min-width: 760px) {
  .header__photo img {
    width: 196px;
    height: 196px;
  }
  .contact__item {
    width: 25%;
    align-items: flex-start;
  }
  .contact__link {
    align-items: flex-start;
  }
}
</style>
