<template>
  <div class="about">
            <div class="loading">
            <div class="blocks" style="--i:1;"></div>
            <div class="blocks" style="--i:2;"></div>
            <div class="blocks" style="--i:3;"></div>
            <div class="blocks" style="--i:4;"></div>
            <div class="blocks" style="--i:5;"></div>
            <div class="blocks" style="--i:6;"></div>
            <div class="blocks" style="--i:7;"></div>
            <div class="blocks" style="--i:8;"></div>
            <div class="blocks" style="--i:9;"></div>
            <div class="blocks" style="--i:10;"></div>
            <div class="blocks" style="--i:11;"></div>
            <div class="blocks" style="--i:12;"></div>
            <div class="blocks" style="--i:13;"></div>
            <div class="blocks" style="--i:14;"></div>
            <div class="blocks" style="--i:15;"></div>
            <div class="blocks" style="--i:16;"></div>
            <div class="blocks" style="--i:17;"></div>
            <div class="blocks" style="--i:18;"></div>
            <div class="blocks" style="--i:19;"></div>
            <div class="blocks" style="--i:20;"></div>
            <h3>Loading</h3>
        </div>
  </div>
</template>

<style>

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: consolas;
}
.about {

  margin-top: 300px;
  margin-left: -897px;
}
@keyframes animationBackgroundColor {
    0%{
        filter: hue-rotate(0deg);
    }
    100%{
        filter: hue-rotate(360deg);
    }
}
.loading{
    position: relative;
    width: 250px;
    height: 250px;
}
.loading .blocks{
    position: absolute;
    width: 8px;
    height: 25px;
    background: #050c09;
    left: 50%;
    background-repeat: 8px;
    transform: rotate(calc(18deg * var(--i)));
    transform-origin: 0 125px;
    animation: animate 1.9s ease-in-out infinite;
    animation-delay: calc(0.05s * var(--i));
}
@keyframes animate {
    0%,50%{
        background: #050c09;
        box-shadow: none;
    }
    50.1%,100%{
        background: #be01fe;
        box-shadow: 0 0 5px #be01fe,
                    0 0 15px #be01fe,
                    0 0 30px #be01fe,
                    0 0 60px #be01fe,
                    0 0 90px #be01fe;
    }
}
h3{
    position:absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 2em;
    letter-spacing: 2px;
    animation: animateText 2s ease-in-out infinite;
    animation-delay: -1s;
}
@keyframes animateText {
    0%,50%{
        color: #050c09;
        text-shadow: none;
    }
    50.1%,100%{
        color: #be01fe;
        text-shadow: 0 0 5px #be01fe,
                    0 0 15px #be01fe;
    }
}
</style>
