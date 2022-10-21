<template>
  <div class="header">
    <div class="cv__container">
      <div class="cv__content">
        <header>
          <div class="header__top">
            <div class="header__photo">
              <img src="" alt="" />
            </div>
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
              <div class="header__hr"></div>
              <div class="header__contacts">
                <div class="contact__item">
                  <h4>Location</h4>
                  <address>Ukraine, Kharkiv</address>
                </div>
                <div class="contact__item">
                  <h4>Phone</h4>
                  <p>+38(099)111-51-91</p>
                </div>
                <div class="contact__item">
                  <a href="#" class="contact__link">
                    <h4>Web</h4>
                    <p>youtube.com</p>
                  </a>
                </div>
                <div class="contact__item">
                  <h4>Email</h4>
                  <p>VoloshinAndy@gmail.com</p>
                </div>
              </div>
            </div>
          </div>
        </header>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>

.cv__container{
  display: flex;
  justify-content: center;
}
.cv__content{
  width: 100%;
  padding: 1.5rem 1.5rem 0;
}

.header__top {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.header__photo {
  position: relative;
  width: 11%;
  width: 200px;
  height: 200px;
  margin-bottom: 24.5px;
}

.header__photo img{
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: yellow;
  border-radius: 50%;
}

.header__content {
  width: 100%;
}

.header__info {
  margin-bottom: 24.5px;
}

.header__info h1{
 text-align: center;
}

.firstname {
  display: block;
  font-weight: 300;
}
.lastname {
  display: block;
  color:#F8BB10;
  font-weight: 700;
  text-transform: uppercase;
}
.header__subinfo {

  font-size: 14px;
}
.header__subinfo h2{
  text-align: center;
  font-weight: 300;
  font-size: 14px;
  padding: 20px 0;
}

header__subinfo h2{
  align-self:center;
}
.header__list {
  display: flex;
  justify-content: center;
}

.fa-github{
  color: #c6c6c6 ;
  border: 2px solid #F8BB10;
  padding: 2px;
  background-color: rgb(237, 237, 237);
  border-radius: 3px;
  border: 2px solid rgb(237, 237, 237);
  text-align: center;
  transition: all .15s linear ;
}

.fa-github:hover{
  color:#F8BB10;
  border: 2px solid rgb(237, 237, 237);
  background: white;
}

.header__hr{
  width: 100%;
  height: 2px;
  background-color:rgb(237, 237, 237) ;
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
  color:#727272;
  font-weight: 600;
  margin-bottom: 8px;
}
.contact__item address{
  font-weight: 400;
  font-style: normal;
}

.contact__link {
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: color .15s linear ;
}

.contact__link:hover{
  color:#F8BB10;
}

@media screen and (min-width:600px) {
  .header__contacts{
    width: 100%;
    flex-direction: row;
    flex-wrap: wrap;
  }

  .contact__item{
    width: 50%;
  }
 }

@media screen and (min-width:760px) {
  .contact__item{
    width: 25%;
  }
  .contact__item{
    align-items:flex-start;
  }
  .contact__link{
    align-items: flex-start;
  }
}


@media screen and (min-width:1024px) {
  .cv__content{
    max-width: 1276px;
    padding: 0;
  }

  .header__top{
    width: 100%;
    height: 100vh;
    flex-direction: row;
    /* width: 100%; */
    /* justify-content: center; */
  }
  .header__photo{
    width: 30%;
    margin: 49px  49px 49px 24px;
    flex: 0 0 auto;
  }

  .header__content{
    width: 70%;
    margin: 49px 24px 49px 49px;
    /* justify-self: flex-start; */
    /* align-self: flex-start; */

  }

}
</style>
