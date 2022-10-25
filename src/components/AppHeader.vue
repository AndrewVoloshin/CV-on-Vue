<template>
  <div class="header">
    <div class="cv__container">
      <div class="cv__content">
        <header>
          <div class="header__top">
            <div class="header__photo-wrap">
            <div class="header__photo">
              <img src="@/assets/HeaderPhoto.jpg" alt="my photo" />
            </div>
    </div>
          <div class="header__content-wrap">
            <div class="header__content">
              <div class="header__info">
                <h1>
                  <span class="firstname">Andrew</span>
                  <span class="lastname">Voloshin</span>
                </h1>
                <div class="header__subinfo">
                  <h2>FrontEnd developer</h2>
                  <ul class="header__list">
                    <li class="header__item">
                      <a href="#" class="header__link">
                        <i class="fa-brands fa-github fa-2x"></i>
                      </a>
                    </li>
                  </ul>
                </div>
              </div>
              <app-contacts></app-contacts>
            </div>
  </div>
          </div>
        </header>
      </div>
    </div>
  </div>
</template>

<script>
import AppContacts from "@/components/AppContacts.vue";
export default {
  components: { AppContacts },
};
</script>

<style lang="scss" scoped>
.cv__container {
  display: flex;
  justify-content: center;
}
.cv__content {
  width: 100%;
  padding: 1.5rem 1.5rem 0;
}

.header__top {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.header__photo {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 24.5px;
}

.header__photo img {
  display: block;
  width: 154px;
  height: 154px;
  background-color: yellow;
  border-radius: 50%;
}

.header__content {
  width: 100%;
}

.header__info {
  margin-bottom: 24.5px;
}

.header__info h1 {
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
.header__subinfo {
  font-size: 14px;
}
.header__subinfo h2 {
  text-align: center;
  font-weight: 300;
  font-size: 14px;
  padding: 20px 0;
}

header__subinfo h2 {
  align-self: center;
}
.header__list {
  display: flex;
  justify-content: center;
}

// .fa-github {
//   color: #c6c6c6;
//   border: 2px solid #f8bb10;
//   padding: 2px;
//   background-color: rgb(237, 237, 237);
//   border-radius: 3px;
//   border: 2px solid rgb(237, 237, 237);
//   text-align: center;
//   transition: all 0.15s linear;
// }

// .fa-github:hover {
//   color: #f8bb10;
//   border: 2px solid rgb(237, 237, 237);
//   background: white;
// }

@media screen and (min-width: 600px) {
}

@media screen and (min-width: 760px) {
  .header__photo img {
    width: 196px;
    height: 196px;
  }
}

@media screen and (min-width: 1024px) {
  .cv__content {
    max-width: 1276px;
    padding: 0;
  }

  .header__top {
    width: 100%;
    // height: 100vh;
    flex-direction: row;
  }
  .header__photo {
    width: 30%;
    padding: 49px 49px 49px 24px;
    flex: 0 0 auto;
  }

  .header__content {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 70%;
    padding: 49px 24px 49px 49px;
    height: 100vh;
  }
  .header__info h1 {
    text-align: left;
  }
  .header__subinfo h2 {
    text-align: left;
  }

  .contacts {
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
  }
}
</style>
