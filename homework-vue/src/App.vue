<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>

      <div class="container">
        <div class="drop" style="--clr:#ff0f5b">
            <div class="content">
                <h2>01</h2>
        <RouterLink to="/">Home</RouterLink>
            </div>
        </div>
        <div class="drop" style="--clr:#be01fe">
            <div class="content">
                <h2>02</h2>
        <RouterLink to="/about">About</RouterLink>
            </div>
        </div>
    </div>

  </header>

  <RouterView />
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap');
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
a{
    text-decoration: none;
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #eff0f4;
}
.container{
  display: flex;
  justify-content: center;
  width:100vw;
  height: 100vh;
    position: relative;
    flex-wrap: wrap;
    padding: 50px 0;
    gap: 40px 60px;
}
.container .drop{
    position: relative;
    width: 200px;
    height: 200px;
    box-shadow: inset 20px 20px 20px rgba(0, 0, 0, .05),
                        25px 35px 20px rgba(0, 0, 0, .05),
                        25px 30px 30px rgba(0, 0, 0, .05),
                        inset -20px -20px 25px rgba(255, 255, 255, .9);
    transition: 0.5s ease-in-out;
    display: flex;
    justify-content: center;
    align-items: center;
}
.container .drop:nth-child(1){
    border-radius: 57% 43% 43% 57% / 43% 43% 57% 57%;
}
.container .drop:nth-child(2){
    border-radius: 61% 39% 52% 48% / 44% 59% 41% 56%;
}
.container .drop:nth-child(3){
    border-radius: 35% 65% 31% 69% / 57% 59% 41% 43%;
}
.container .drop:hover{
    border-radius: 50%;
}
.container .drop::before{
    content: '';
    position: absolute;
    top: 50px;
    left: 85px;
    width: 35px;
    height: 35px;
    background: #fff;
    border-radius: 50%;
    opacity: 0.9;
}
.container .drop::after{
    content: '';
    position: absolute;
    top: 90px;
    left: 110px;
    width: 15px;
    height: 15px;
    background: #fff;
    border-radius: 50%;
    opacity: 0.9;
}
.container .drop .content{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    padding: 5px;
    gap: 5px;
    margin-left: 0;
}
.container .drop .content h2{
    position: relative;
    width: 80px;
   height: 80px;
    background: #eff0f4;
    border-radius: 50%;
    box-shadow: inset 2px 5px 10px rgba(0, 0, 0, 0.1),
                inset -2px -5px 10px rgba(255, 255, 255, 1),
                15px 15px 10px rgba(0, 0, 0, .05),
                15px 10px 15px rgba(0, 0, 0, .025);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 2em;
    color: var(--clr);
}
.container .drop .content a{
    position: relative;
    padding: 10px 25px;
    background-color: var(--clr);
    color: #fff;
    border-radius: 25px;
    font-weight: 500;
    text-shadow: 0 2px 2px rgba(0, 0, 0, .25);
    opacity: 0.75;
    transition: 0.5s;
}
.container .drop .content a:hover{
    opacity: 1;
}
</style>