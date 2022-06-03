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
    <CarLine name="bmw 335i e92" :features="[{title:'cylindrée', value: '3000cc'},{title:'Motorisation',value:'6 cylindres en ligne (turbo)'},{title:'puissance',value: '306cv'},{title:'0 à 100',value:'5,6 sec'}]" image="https://media.schmiedmann.com/media/79312/bmw_335i_e92_by_schmiedmann_finland_hdr03.jpg?maxwidth=1024&maxheight=768"></CarLine>
    
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
