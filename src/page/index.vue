<template>
  <div>
    <section id="main">
      <nav>
        <div class="container-nav">
          <div
            style="
              border: 2px solid #d08210;
              color: white;
              padding: 10px;
              border-radius: 5px;
              max-width: 250px;
              font-size: 0.5em;
              text-align: center;
              letter-spacing: 5px;
            "
          >
            JAKKRIT SINGSAT
          </div>
          <div class="social-box">
            <i class="fab fa-facebook"></i>
            <i class="fab fa-instagram"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-youtube"></i>
          </div>
        </div>
      </nav>
      <div class="container">
        <div class="text-header">
          <div class="logo-profile-mobile"></div>
          <div>
            <h1 class="title">
              I'm <font color="#d08210">Jakkrit</font> Singsat
            </h1>
            <p
              style="
                margin-top: 10px;
                color: white;
                letter-spacing: 3px;
                font-size: 1.5em;
              "
            >
              Frontend Developer
            </p>
            <p
              style="
                font-size: 1em;
                max-width: 900px;
                text-transform: lowercase;
                color: white;
                margin-top: 5px;
              "
              class="introduction"
            >
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi
              voluptates, nemo soluta quasi veritatis doloribus similique
              voluptatum quas repellat cupiditate! Aliquam eaque accusantium
              sequi explicabo fuga, et iure unde sed?
            </p>
            <button
              style="
                width: 200px;
                height: 50px;
                border: 2px solid white;
                background-color: transparent;
                color: white;
                font-size: 1.5em;
                border-radius: 5px;
                margin-top: 30px;
              "
            >
              RESUME
            </button>
          </div>
          <div class="logo-profile"></div>
        </div>
        <div class="my-skill">
          <div>
            <h1 class="title">MY<font color="#d08210">skills</font> </h1>
          </div>
        </div>
        <div class="skills-detail">
          <div class="skill-item">
            <img src="../assets/img/html.png">
          </div>
          <div class="skill-item">
            <img src="../assets/img/css.png">
          </div>
          <div class="skill-item">
            <img src="../assets/img/vue.png">
          </div>
          <div class="skill-item">
            <img src="../assets/img/node.png">
          </div>
              <div class="skill-item">
            <img src="../assets/img/js.png">
          </div>
          <div class="skill-item">
            <img src="../assets/img/git.png">
          </div>
        </div>
        <div class="container-box">
          <div class="item-box">
            <div class="item-body1"></div>
            <div class="item-title">
              <span>Landing page</span>
            </div>
          </div>
          <div class="item-box">
            <div class="item-body2"></div>
            <div class="item-title">
              <span>Web Application</span>
            </div>
          </div>
          <div class="item-box">
            <div class="item-body3"></div>
            <div class="item-title">
              <span>Application</span>
            </div>
          </div>
        </div>
      </div>
      <DialogSlick :isActiveDialog="isActiveDialog"/>
    </section>
  </div>
</template>
<script>
  import DialogSlick from '@/components/DialogSlick.vue';
export default {
  component:{
    DialogSlick
  },
  data() {
    return {
      isActiveDialog:false,
    }
  },
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans:wght@400;700&display=swap');
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'Noto Sans', sans-serif;
}
@media (max-width: 320px) {
  .my-skill .title{
    font-size: 2.5em!important;
  }
  .introduction {
    display: none;
  }
  .logo-profile-mobile {
    margin-top: 15px;
    width: 150px !important;
    height: 150px !important;
    background-image: url('../assets/img/IMG_4957.jpg') !important;
    background-repeat: no-repeat !important;
    background-position: center !important;
    background-size: cover !important;
    border-radius: 50% !important;
  }
  .social-box {
    font-size: 25px !important;
  }
  .text-header {
    padding: 120px 50px !important;
  }
  .text-header .title {
    margin-top: 15px;
    font-size: 2.5em !important;
  }
  .text-header p {
    font-size: 1.5em !important;
  }
}
@media (max-width: 775px) {
  .container-nav div {
    margin-top: 20px;
  }
  .container-nav {
    flex-direction: column;
  }
  .text-header {
    text-align: center;
  }
  .container-box {
    flex-wrap: nowrap !important;
    flex-direction: column;
    padding: 0 20px !important;
  }
  .container-box .item-box {
    width: 100% !important;
    margin-top: 15px !important;
  }
  #main,
  .container {
    height: auto !important;
  }
}
@media (max-width: 600px) {
  .skills-detail{
    flex-direction: column!important;
    height: 670px!important;
    align-items: center!important;
    justify-content: space-around!important;
  }
}
@media (max-width: 1200px) {
  .text-header .title{
    margin-top:15px!important;
  }
  .my-skill{
    justify-content: center!important;
  }
  .text-header {
    flex-direction: column;
    text-align: center;
  }
  .logo-profile-mobile {
    background-image: url('../assets/img/IMG_4957.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    width: 300px;
    height: 300px;
    border-radius: 50%;
  }
  .logo-profile {
    display: none;
  }
  .introduction{
  padding:0px 30px!important;
}
}
.item-box{
  cursor: pointer;
  transition: 0.3s;
}
.item-box:hover{
  transform: scale(0.95);
}
.text-header {
  padding-top: 3rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.social-box {
  font-size: 30px;
  color: white;
  opacity: 0.5;
}
.social-box i{
  margin-right: 10px;
}
.social-box i:last-child{
  margin-right: 0px;
}
nav a {
  text-decoration: none;
}
nav {
  width: 100%;
  background-color: transparent;
  height: 80px;
  position: relative;
  left: 0;
  top: 0;
  z-index: 99;
}
.my-skill {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  margin-top:25px;
}
nav ul {
  list-style: none;
  display: flex;
}
li a {
  color: white;
  margin-left: 20px;
  transition: 0.4;
}
li a:hover {
  border-bottom: 5px solid white;
}
.item-box .item-body1 {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/img/1.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.item-box .item-body2 {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/img/1.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.item-box .item-body3 {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/img/1.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
/* .item-box .item-body4 {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/img/1.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.item-box .item-body5 {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/img/1.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
} */
.item-box .item-body6 {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/img/1.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.item-box .item-title {
  width: 100%;
  height: 50px;
  position: absolute;
  bottom: 50%;
  left: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: calabri;
  color: white;
  letter-spacing: 5px;
  font-weight: 100;
}
.container-box .item-box {
  width: 32%;
  height: 400px;
  margin: 5px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: white;
}
.container-box {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 50px 10px;
}
.container h1 {
  font-size: 4em;
  text-transform: uppercase;
  color: white;
}
.container p {
  font-size: 3em;
  text-transform: uppercase;
}
.container span {
  font-size: 1.5em;
  text-transform: uppercase;
}
.container-nav {
  max-width: 1300px;
  margin: 0 auto;
  font-size: 25px;
  font-family: calabri;
  padding: 0 10px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100%;
  text-transform: uppercase;
  font-weight: 100;
}
.container {
  max-width: 1300px;
  margin: 0 auto;
  font-size: 16px;
  font-family: calabri;
  position: relative;
}
.item-body img {
  width: 300px;
  padding: 20px;
}
.social {
  width: 100%;
  position: absolute;
  bottom: 0;
  right: 0;
  height: 50px;
  display: flex;
  justify-content: flex-end;
  padding: 0px 10px;
}
.my-skill .title{
    font-size: 2em;
}
.title {
  line-height: 50px;
  margin: 0px;
  font-weight: 700;
  letter-spacing: 5px!important;
  font-size: 2.5em !important;
}
#main {
  width: 100%;
  background-image: linear-gradient(
      rgba(22, 22, 22, 0.9),
      rgba(20, 20, 20, 0.5)
    ),url('../assets/img/IMG_4961.jpg');
  background-repeat: no-repeat;
  background-position: center bottom;
  background-size: cover;
  position: relative;
}
.logo-profile {
  background-image: url('../assets/img/IMG_4957.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  width: 250px;
  height: 250px;
  border-radius: 50%;
}
.skills {
  display: flex;
  align-items: center;
}
.skills-detail{
  margin-top:35px;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  height: 300px;
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.5));
}
.skill-item img{
  width:100px;
  height: 100px;
  filter: invert(100%);
  -webkit-filter: invert(100%);
}
</style>