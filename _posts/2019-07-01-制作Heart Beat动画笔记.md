---
layout: tag
title: Heart Beat
date: 2019-07-01
tags:
     - SVG制作
---

## 如何制作心跳的动图？？
 <!--more-->
 
 首先我们先找一个SVG图
 
 ```
 <svg t="1561972001885" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1710" width="200" height="200">
 <path d="M755.2 64c-107.616 0-200.256 87.552-243.168 179.008-42.944-91.456-135.584-179.008-243.232-179.008-148.384 0-268.8 120.448-268.8 268.832 0 301.856 304.512 380.992 512.032 679.424 196.16-296.576 511.968-387.2 511.968-679.424 0-148.384-120.416-268.832-268.8-268.832z" p-id="1711" fill="#d81e06"></path></svg>
 ```
 
 <svg t="1561972001885" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1710" width="200" height="200"><path d="M755.2 64c-107.616 0-200.256 87.552-243.168 179.008-42.944-91.456-135.584-179.008-243.232-179.008-148.384 0-268.8 120.448-268.8 268.832 0 301.856 304.512 380.992 512.032 679.424 196.16-296.576 511.968-387.2 511.968-679.424 0-148.384-120.416-268.832-268.8-268.832z" p-id="1711" fill="#d81e06"></path></svg>
 
 并且让它放在中间用到center元素
 
 再添加CSS
 
 变成
 
 <center>
<div class="heart" style="width: 50%" >
<svg t="1561972001885" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1710" width="200" height="200"><path d="M755.2 64c-107.616 0-200.256 87.552-243.168 179.008-42.944-91.456-135.584-179.008-243.232-179.008-148.384 0-268.8 120.448-268.8 268.832 0 301.856 304.512 380.992 512.032 679.424 196.16-296.576 511.968-387.2 511.968-679.424 0-148.384-120.416-268.832-268.8-268.832z" p-id="1711" fill="#d81e06"></path></svg> 
</div>
</center>

<style>
#heart { 
  position: absolute;
  top:50%;
  left:50%;
  width: 100px; 
  height: 90px;
  margin:-50px -45px;
  -webkit-transition:all 1s ease;
  -webkit-animation: latidoslatinosurbanosemergenteshiphophermanobrother 1s infinite;
} 
#heart:before, #heart:after { 
  position: absolute; 
  content: ""; 
  left: 50px; 
  top: 0; 
  width: 50px; 
  height: 80px; 
  background: hsl(0,50%,50%); 
  border-radius: 50px 50px 0 0; 
  -webkit-transform: rotate(-45deg); 
  -moz-transform: rotate(-45deg); 
  -ms-transform: rotate(-45deg); 
  -o-transform: rotate(-45deg); 
  transform: rotate(-45deg); 
  -webkit-transform-origin: 0 100%; 
  -moz-transform-origin: 0 100%; 
  -ms-transform-origin: 0 100%; 
  -o-transform-origin: 0 100%; 
  transform-origin: 0 100%; 
} 
#heart:after { 
  left: 0; 
  -webkit-transform: rotate(45deg); 
  -moz-transform: rotate(45deg); 
  -ms-transform: rotate(45deg); 
  -o-transform: rotate(45deg); 
  transform: rotate(45deg); 
  -webkit-transform-origin: 100% 100%; 
  -moz-transform-origin: 100% 100%; 
  -ms-transform-origin: 100% 100%; 
  -o-transform-origin: 100% 100%; 
  transform-origin :100% 100%; 
} 

/* HEARTBEAT ANIMATION BY Mi1o */
@-webkit-keyframes latidoslatinosurbanosemergenteshiphophermanobrother {
  0% { -webkit-transform: scale(1); }
  8% { -webkit-transform: scale(0.7);  }
  17% { -webkit-transform: scale(1.5); }
  25% { -webkit-transform: scale(0.7); }
  87.5% { -webkit-transform: scale(0.7); }
  100%  { -webkit-transform: scale(1); }
}
</style>
 
 
