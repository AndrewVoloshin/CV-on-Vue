<template>
  <div class="toggle-dark-light">
    <button
      type="button"
      class="toggle__button"
      :class="{ 'toggle__button--active': isDark }"
      @click="toggleTheme"
    >
      
      <span v-if="isDark" class="toggle__icon" :class="{ 'toggle__icon--light': isDark }"
        >Dark</span
      >
      <span v-else class="toggle__icon" :class="{ 'toggle__icon--light': isDark }"
        >Light</span
      >
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isDark: false,
    };
  },
  methods: {
    toggleTheme() {
      this.isDark = !this.isDark;
      console.log("click herer54");
      document.documentElement.style.setProperty("--sub-bg-color", "red");
    },
  },
};
</script>

<style land="scss" scoped>
.toggle-dark-light {
  position: fixed;
  bottom: 12px;
  right: 12px;
  width: 40px;
  height: 40px;
  z-index: 99;
}

.toggle__button {
  position: absolute;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #f8bb10;
  border-radius: 50%;
  box-shadow: 0 4px 8px 0 #11111180;
}

</style>
