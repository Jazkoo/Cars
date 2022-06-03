<template>
  <div>

    

<div class="page">
  <header tabindex="0"><h1>BMW</h1></header>
  <div id="nav-container">
    <div class="bg"></div>
    <div class="button" tabindex="0">
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
    </div>
    <div id="nav-content" tabindex="0">
      <ul>
        <li><a href="#/">Home</a></li>
        <li><a href="#0">Services</a></li>
        <li><a href="#0">Blog</a></li>
        <li><a href="#0">About</a></li>
        <li><a href="/contact">Contact</a></li>
        <li class="small"><a href="#0">Facebook</a><a href="#0">Instagram</a></li>
      </ul>
    </div>
  </div>

  <main>
    <div class="content">

    <CarLine name="bmw M3 e36" :features="[{title:'cylindrée', value: '3200cc'},{title:'Motorisation',value:'6 cylindres en ligne'},{title:'puissance',value: '321cv'},{title:'0 à 100',value:'5,5 sec'}]" image="https://delessencedansmesveines.com/wp-content/uploads/2018/07/DLEDMV-2K18-BMW-E36-Cab-AC-Schnitzer-Mircea-Lu%C5%A3uc-01.jpg" />
    <CarLine name="bmw M5 F10" :features="[{title:'cylindrée', value: '4400cc'},{title:'Motorisation',value:'V8'},{title:'puissance',value: '575cv'},{title:'0 à 100',value:'4,3 sec'}]" image="https://w0.peakpx.com/wallpaper/315/700/HD-wallpaper-bmw-m5-f10-exterior-gray-matt-m5-tuning-f10-bronze-wheels-m-package-german-cars-bmw.jpg"/>
    <CarLine name="bmw 335i e92" :features="[{title:'cylindrée', value: '3000cc'},{title:'Motorisation',value:'6 cylindres en ligne (turbo)'},{title:'puissance',value: '306cv'},{title:'0 à 100',value:'5,6 sec'}]" image="data:image/jpeg;base64,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"
  
  </div>
  </main>
</div>


  </div>

</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
<style>
h2{
  color:white;
  font-weight: bold;
  font-family:arial;
  font-size:24px;
}
h1{

  color:white;
  font-weight: bold;
  font-family:arial;
  font-size:30px
}
 

 table tr td,table, table tr{
   border-collapse:collapse;
   border: 1px solid #000;
   margin:0;
   padding:10px;
 }
table tr td {
  text-align:left;
  font-weight:bold;
  text-decoration: underline ;
  text-transform: uppercase ;
  background-color: blue ;
  width:20%;}

table tr td:last-child {
  background-color: lightblue ;
  width:50%;
  text-align:center;
  }

@import url('https://fonts.googleapis.com/css?family=Encode+Sans+Condensed:400,600');

* {
  outline: none;
}

strong {
  font-weight: 600;
}

.page {
  width: 100%;
  height: 100vh;
  background: #fdfdfd;
  font-family: 'Encode Sans Condensed', sans-serif;
  font-weight: 600;
  letter-spacing: .03em;
  color:black;
}

header {
  padding-top: 10px;
  display: flex;
  position: relative;
  width: 100%;
  height: 100px;
  background: #000;
  color:#fff;
  justify-content: center;
  align-items: center;
  -webkit-tap-highlight-color: rgba(0,0,0,0);
}

main {
  padding: 70px 20px 0;
  display: flex;
  flex-direction: column;
  height: 100%;
}


main h2 span {
  color: #BF7497;
}

main p {
  line-height: 1.5;
  font-weight: 200;
  margin: 20px 0;
}

main small {
  font-weight: 300;
  color: #888;
}

#nav-container {
  position: fixed;
  height: 100vh;
  width: 100%;
  pointer-events: none;
}
#nav-container .bg {
  position: absolute;
  top:70px;
  left: 0;
  width: 100%;
  height: calc(100% - 70px);
  visibility: hidden;
  opacity: 0;
  transition: .3s;
  background: #000;
}
#nav-container:focus-within .bg {
  visibility: visible;
  opacity: .6;
}
#nav-container * {
  visibility: visible;
}

.button {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  z-index: 1;
  -webkit-appearance: none;
  border: 0;
  background: transparent;
  border-radius: 0;
  height: 70px;
  width: 30px;
  cursor: pointer;
  pointer-events: auto;
  margin-left: 25px;
  touch-action: manipulation;
  -webkit-tap-highlight-color: rgba(0,0,0,0);
}
.icon-bar {
  display: block;
  width: 100%;
  height: 3px;
  background: #aaa;
  transition: .3s;
}
.icon-bar + .icon-bar {
  margin-top: 5px;
}

#nav-container:focus-within .button {
  pointer-events: none;
}
#nav-container:focus-within .icon-bar:nth-of-type(1) {
  transform: translate3d(0,8px,0) rotate(45deg);
}
#nav-container:focus-within .icon-bar:nth-of-type(2) {
  opacity: 0;
}
#nav-container:focus-within .icon-bar:nth-of-type(3) {
  transform: translate3d(0,-8px,0) rotate(-45deg);
}

#nav-content {
  margin-top: 70px;
  padding: 20px;
  width: 70%;
  max-width: 300px;
  position: absolute;
  top: 0;
  left: 0;
  height: calc(100% - 70px);
  background: #ececec;
  pointer-events: auto;
  -webkit-tap-highlight-color: rgba(0,0,0,0);
  transform: translateX(-100%);
  transition: transform .3s;
  will-change: transform;
  contain: paint;
}

#nav-content ul {
  height: 100%;
  display: flex;
  flex-direction: column;
  background-color: black;

}

#nav-content li a {
  padding: 10px 5px;
  display: block;
  text-transform: uppercase;
  transition: color .1s;
}

#nav-content li a:hover {
  color: #BF7497;
}

#nav-content li:not(.small) + .small {
  margin-top: auto;
}

.small {
  display: flex;
  align-self: center;
}

.small a {
  font-size: 12px;
  font-weight: 400;
  color: #888;
}
.small a + a {
  margin-left: 15px;
}

#nav-container:focus-within #nav-content {
  transform: none;
}


.content{
  padding:20px;
  display:flex;
  flex-direction:column;
  align-content: center;
  flex-wrap:wrap;



  
  /* Large */
.navigation {
  display: flex;
  flex-flow: row wrap;
  /* This aligns items to the end line on main-axis */
  justify-content: flex-end;
}

/* Medium screens */
@media all and (max-width: 800px) {
  .navigation {
    /* When on medium sized screens, we center it by evenly distributing empty space around items */
    justify-content: space-around;
  }
}

/* Small screens */
@media all and (max-width: 500px) {
  .navigation {
    /* On small screens, we are no longer using row direction but column */
    flex-direction: column;
  }
}

}



* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html, body {
  height: 100%;
}

a,
a:visited,
a:focus,
a:active,
a:link {
  text-decoration: none;
  outline: 0;
}

a {
  color: currentColor;
  transition: .2s ease-in-out;
}

h1, h2, h3, h4 {
  margin: 0;
}

ul {
  padding: 0;
  list-style: none;
}

img {
  
}

</style>
