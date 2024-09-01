<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="bg newFont">
    <div class="row1"></div>
    <div class="row2">
      <div class="col1">
        <div>Light and Dark Mode Coming Soon</div>
      </div>
      <div class="content">
        <div class="menu">
          <div>
            <div class="name" @click="$router.push('/')">Chance Stribling</div>
            <div class="title">Designer and Developer</div>
          </div>
          <div>
            <div class="menu-text cursor-pointer glow" @click.native="$router.push('/')">Home</div>
            <div class="menu-text cursor-pointer glow" @click.native="$router.push('/technologies')">Technologies</div>
            <div class="menu-text cursor-pointer glow" @click.native="$router.push('/portfolio')">Portfolio</div>
            <div class="menu-text cursor-pointer glow">Contact</div>
          </div>
        </div>
        <div class="rv">
          <RouterView />
        </div>
      </div>
      <div class="col3"></div>
    </div>
    <div class="row3">
      <div class="col4"></div>
      <div class="col5">Designed by Chance Stribling</div>
      <div class="col6"></div>
    </div>
  </div>
</template>

<style scoped>
.bg {
  background-color: black;
  position: absolute;
  color: white;
  height: 100dvh;
  width: 100svw;
}
.row1 {
  height: 4%;
}
.row2 {
  display: flex;
  flex-direction: row;
  height: 92%;
}
.row3 {
  height: 4%;
  display: flex;
}
.col1 {
  height: 100%;
  width: 2%;
  min-width: 20px;
  writing-mode: vertical-lr;
  transform: rotate(180deg);
}
.content {
  height: 100%;
  width: 95%;
  border-style: solid;
  border-width: 1%;
  border-color: white;
}
.col3 {
  height: 100%;
  width: 2%;
  min-width: 20px;
}
.col4 {
  width: 2%;
  min-width: 20px;
}
.col5 {
  width: 96%;
}
.col6 {
  width: 2%;
  min-width: 20px;
}
.menu {
  position: absolute;
  height: 300px;
  width: fit-content;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.newFont {
  font-family: 'Cutive Mono', monospace;
  font-weight: 400;
  font-style: normal;
}
.name {
  font-size: 46px;
}
.title {
  font-size: 24px;
}
.rv {
  height: 100%;
  z-index: 2;
}
.menu-text{
  font-size: 20px;
  margin-top: 20px;
}
.glow {
  color: #fff;
  -webkit-animation: glow 1s ease-in-out infinite alternate;
  -moz-animation: glow 1s ease-in-out infinite alternate;
  animation: glow 1s ease-in-out infinite alternate;
}

@-webkit-keyframes glow {
  from {
    text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px  #ececec , 0 0 40px  #ececec , 0 0 50px  #ececec , 0 0 60px  #ececec , 0 0 70px  #ececec ;
  }
  to {
    text-shadow: 0 0 20px #fff, 0 0 30px #ffffff, 0 0 40px #ffffff, 0 0 50px #ffffff, 0 0 60px #ffffff, 0 0 70px #ffffff, 0 0 80px #ffffff;
  }
}
@keyframes glow {
  from {
    text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px  #ececec , 0 0 40px  #ececec , 0 0 50px  #ececec , 0 0 60px  #ececec , 0 0 70px  #ececec ;
  }
  to {
    text-shadow: 0 0 20px #fff, 0 0 30px #ffffff, 0 0 40px #ffffff, 0 0 50px #ffffff, 0 0 60px #ffffff, 0 0 70px #ffffff, 0 0 80px #ffffff;
  }
}

@media only screen and (max-width: 1000px) {
  .name {
    font-size: 16px;
    font-weight: bold;
  }
  .title {
    font-size: 10px;
  }
  .bg {
    width: 100dvw;
  }
  .menu-text{
    font-size: 16px;
  }
}
</style>
