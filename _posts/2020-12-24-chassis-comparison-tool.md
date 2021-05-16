---
layout: default
title: Vehicle chassis comparison tool
displayTitle: "Vehicle chassis comparison tool"
date: 2020-12-24 10:36:00
excerpt: > 
  A tool to help compare common enthusiast car chassis sizes, side by side
metaDescription: A tool to help compare common enthusiast car chassis sizes, side by side
metaKeywords: automotive, cars
metaOgType: "article"
image: /static/images/2020-12-20-subaru-vin-plate-location.jpg
metaImage: /static/images/2020-12-20-subaru-vin-plate-location.jpg
author: "0xADADA"
tags: [motorsports]
license: cc-by-nc-sa
style: |
  body {
    position: relative;
    height: 100vh;
    margin: 0;
    padding: 0;
  }
  header, .article-footer, .footer {
    display: none;
  }
  
  .labels {
    position: fixed;
    bottom: 10px;
    align-items: center;
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    
  }
  label {
    border-radius: 4px;
    border: 1px solid #dbdbdb;
    padding: 0.25em;
    margin: 0.125em;
  }
  .preview {
    transform: scale(0.15) translate(-250%, 25%); 
    position: relative;
  }
  .vehicle {
    border: 10px solid red;
    position: absolute;
    font-size: 172px;
    font-family: sans-serif;
    appearance: none;
    background: transparent;
    opacity: 0.25;
    text-align: center;
    transition: background-color 500ms ease;
  }
  .vehicle:focus {
    opacity: 0.95;
    z-index: 10;
    background-color: white;
  }
  
  .na {
    height: 2265px;
    width: 1675px;
    color: rgb(21%, 56%, 79%);
    border-color: rgb(21%, 56%, 79%);
  }
  .ae86 {
    border-color: rgb(63%, 43%, 46%);
    color: rgb(63%, 43%, 46%);
    width: 1625px;
    height: 2400px;
  }
  .p930 {
    border-color: rgb(68%, 67%, 47%);
    color: rgb(68%, 67%, 47%);
    width: 1775px;
    height: 2272px;
  }
  .ap2 {
    width: 1750px;
    height: 2400px;
    border-color: rgb(61%, 34%, 58%);
    color: rgb(61%, 34%, 58%);
  }
  .fc {
    border-color: rgb(73%, 32%, 29%);
    color: rgb(73%, 32%, 29%);
    height: 2431px;
    width: 1689px;
  }
  .fd {
    border-color: rgb(90%, 16%, 84%);
    color: rgb(90%, 16%, 84%);
    height: 2446px;
    width: 1760px;
  }
  .j29 {
    color: rgb(99%, 33%, 52%);
    border-color: rgb(99%, 33%, 52%);
    height: 2470px;
    width: 1865px;
  }
  .s13 {
    border-color: rgb(68%, 34%, 29%); 
    color: rgb(68%, 34%, 29%);
    height: 2474px;
    width: 1689px;
  }
  .ce {
    border-color: rgb(50%, 26%, 78%);
    color: rgb(50%, 26%, 78%); 
    height: 2510px;
    width: 1695px;
  }
  .gc {
    border-color: rgb(87%, 16%, 66%);
    color: rgb(87%, 16%, 66%); 
    height: 2520px;
    width: 1690px;
  }
  .s15 {
    width: 1695px;
    height: 2525px;
    border-color: rgb(48%, 57%, 3%);
    color: rgb(48%, 57%, 3%);
  }
  .s14 {
    width: 1730px;
    height: 2525px;
    border-color: rgb(48%, 57%, 3%);
    color: rgb(48%, 57%, 3%);
  }
  .gd {
    width: 1730px;
    height: 2525px;
    color: orange;
    border-color: orange;
  }
  .a80 {
    border-color: rgb(85%, 39%, 45%);
    color: rgb(85%, 39%, 45%);
    height: 2550px;
    width: 1810px;
  }
  .z370 {
    height: 2550px;
    width: 1850px;
    color: rgb(36%, 50%, 71%);
    border-color: rgb(36%, 50%, 71%);
  }
  .e30 {
    width: 1680px;
    height: 2562px;
    color: black;
    border-color: black;
  }
  .zc6 {
    border-color: rgb(17%, 82%, 68%);
    color: rgb(17%, 82%, 68%);
    width: 1760px;
    height: 2570px;
  }
  .r32 {
    border-color: rgb(58%, 79%, 21%);
    color: rgb(58%, 79%, 21%);
    width: 1755px;
    height: 2615px;
  }
  .z350 {
    height: 2649px;
    width: 1816px;
    border-color: rgb(46%, 15%, 88%);
    color: rgb(46%, 15%, 88%);
  }
  .cz {
    border-color: rgb(25%, 91%, 61%);
    color: rgb(25%, 91%, 61%);
    height: 2650px;
    width: 1810px;
  }
  .r34 {
    border-color: rgb(20%, 60%, 14%);
    color: rgb(20%, 60%, 14%);
    width: 1785px;
    height: 2665px;
  }
  .e36 {
    border-color: rgb(86%, 100%, 9%);
    color: rgb(86%, 100%, 9%);
    width: 1710px;
    height: 2700px;
  }
  .r33 {
    border-color: rgb(93%, 67%, 38%);
    color: rgb(93%, 67%, 38%);
    width: 1780px;
    height: 2720px;
  }
  .e46 {
    border-color: rgb(50%, 58%, 77%);
    color: rgb(50%, 58%, 77%);
    height: 2720px;
    width: 1780px;
  }
  .xc10 {
    border-color: rgb(59%, 90%, 26%);
    color: rgb(59%, 90%, 26%);
    width: 1845px;
    height: 2730px;
  }
  .r35 {
    border-color: rgb(31%, 31%, 55%);
    color: rgb(31%, 31%, 55%);
    height: 2780px;
    width: 1895px;
  }
  .f80 {
    border-color: rgb(59%, 90%, 26%);
    color: rgb(59%, 90%, 26%);
    width: 1877px;
    height: 2812px;
  }
---


<div class="labels">
  <label for="na">NA</label>
  <label for="p930">930</label>
  <label for="ae86">AE86</label>  
  <label for="ap2">AP2</label>
  <label for="fc">FC</label>
  <label for="fd">FD</label>
  <label for="j29">J29</label>
  <label for="s13">S13</label>
  <label for="ce">CE</label>
  <label for="gc">GC</label>
  <label for="s15">S15</label>
  <label for="s14">S14</label>
  <label for="gd">GD</label>
  <label for="a80">A80</label>
  <label for="z34">Z34</label>
  <label for="e30">E30</label>
  <label for="zc6">ZC6</label>
  <label for="r32">R32</label>
  <label for="z350">Z33</label>
  <label for="cz">CZ</label>
  <label for="r34">R34</label>
  <label for="e36">E36</label>
  <label for="r33">R33</label>
  <label for="e46">E46</label>
  <label for="xc10">XC10</label>
  <label for="r35">R35</label>
  <label for="f80">F80</label>

</div>

<div class="preview">
  <input id="na" class="vehicle na" readonly value="Maza Miata (NA)">
  <input id="p930" class="vehicle p930" readonly value="Porsche 911 (930)">
  <input id="ae86" class="vehicle ae86" readonly value="Toyota AE86">
  <input id="ap2" class="vehicle ap2" readonly value="Honda S2000 (AP2)">
  <input id="fc" class="vehicle fc" readonly value="Mazda RX-7 (FC)">
  <input id="fd" class="vehicle fd" readonly value="Mazda RX-7 (FD)">
  <input id="j29" class="vehicle j29" readonly value="Toyota Supra (J29)">
  <input id="s13" class="vehicle s13" readonly value="Nissan 180SX (S13)">
  <input id="ce" class="vehicle ce" readonly value="Mitsubishi EVOII (CE)">
  <input id="gc" class="vehicle gc" readonly value="Subaru WRX (GC)">
  <input id="s15" class="vehicle s15" readonly value="Nissan Silvia (S15)">
  <input id="gd" class="vehicle gd" readonly value="Subaru WRX (GD)">
  <input id="s14" class="vehicle s14" readonly value="Nissan Silvia (S14)">
  <input id="a80" class="vehicle a80" readonly value="Toyota Supra(A80)">
  <input id="z34" class="vehicle z370" readonly value="Nissan 370Z (Z34)">
  <input id="e30" class="vehicle e30" readonly value="BMW M3 (E30)">
  <input id="zc6" class="vehicle zc6" readonly value="Subaru BRZ (ZC6)">
  <input id="r32" class="vehicle r32" readonly value="Nissan GT-R (R32)">
  <input id="z350" class="vehicle z350" readonly value="Nissan 350Z (Z33)">
  <input id="cz" class="vehicle cz" readonly value="Mitsubishi EVO X (CZ)">
  <input id="r34" class="vehicle r34" readonly value="Nissan GT-R (R34)">
  <input id="e36" class="vehicle e36" readonly value="BMW M3 (E36)">
  <input id="r33" class="vehicle r33" readonly value="Nissan GT-R (R33)">
  <input id="e46" class="vehicle e46" readonly value="BMW M3 (E46)">
  <input id="xc10" class="vehicle xc10" readonly value="Lexus RC (XC10)">
  <input id="r35" class="vehicle r35" readonly value="Nissan GT-R  (R35)">
  <input id="f80" class="vehicle f80" readonly value="BMW M3 (F80)">
</div>
