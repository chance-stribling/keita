<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="bg">
    <div class="row1"></div>
    <div class="row2">
      <div class="col1">
        <div>Light and Dark Mode Coming Soon</div>
      </div>
      <div class="content">
        <div class="menu">
          <div>
            <div class="text-h3 name" @click="$router.push('/')">Chance Stribling</div>
            <div class="text-p">Designer and Developer</div>
          </div>
          <div>
            <div class="text-p cursor-pointer" @click.native="$router.push('/')">Home</div>
            <div class="text-p cursor-pointer" @click.native="$router.push('/technologies')">Technologies</div>
            <div class="text-p cursor-pointer">Portfolio</div>
            <div class="text-p cursor-pointer">Contact</div>
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
  background-color: green;
  position: absolute;
  color: white;
  height: 100vh;
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
  width: 2vw;
  min-width: 20px;
  writing-mode: sideways-lr;
}
.content {
  height: 100%;
  width: 96vw;
  border-style: solid;
  border-width: 0.5px;
  border-color: white;
}
.col3 {
  height: 100%;
  width: 2vw;
  min-width: 20px;
}
.col4 {
  width: 2vw;
  min-width: 20px;
}
.col5 {
  width: 96vw;
}
.col6 {
  width: 2vw;
  min-width: 20px;
}
.menu {
  position: absolute;
  height: 300px;
  width: 500px;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.rv {
  height: 100%;
  z-index: 2;
}
@media only screen and (max-width: 1000px) {
.name{
  font-size: 30px !important;
}
.content{
  width: 92vw;
}
} 
</style>
