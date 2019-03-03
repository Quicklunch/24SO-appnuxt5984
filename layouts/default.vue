<template>
  <div>
    <TheHeader @sidenavToggle="displaySidenav = !displaySidenav" />
    <TheSidenav
     :show="displaySidenav"   
     @close="displaySidenav = false"/>
     <div class="content">
         <nuxt />
     </div> 
  </div>
</template>

<script>
import TheHeader from '@/components/Navigation/TheHeader' 
import TheSidenav from '@/components/Navigation/TheSidenav' 

    export default {
        components: {
            TheHeader,
            TheSidenav
        },
        data() {
            return {
                displaySidenav: false
            }
        }
    }
</script>

<style>
html, input, textarea, select, button, button, ul li {
    font-family: 'Roboto', sans-serif;
}

span {
    font-family: Roboto;
    font-style: normal;
    font-weight: normal;
    line-height: 36px;
    font-size: 20px;
    color: #112233;
}

h1 {
    font-style: normal;
    font-weight: bold;
    line-height: 64px;
    font-size: 48px;
    text-align: center;
}

h2 {
    font-style: normal;
    font-weight: bold;
    line-height: 43px;
    font-size: 36px;
    text-align: center;
}

h4 {
    font-style: normal;
    font-weight: 500;
    line-height: 36px;
    font-size: 24px;
    color: #445566;
}

p {
    font-style: normal;
    font-weight: normal;
    line-height: 30px;
    font-size: 16px;
    color: #445566;
    }

h5 {
    font-family: Roboto;
    font-style: normal;
    font-weight: bold;
    line-height: 32px;
    font-size: 16px;
    color: #112233;
}
.content {
    padding-right: 5%;
    padding-left: 5%;
    width: 100%;
    background: #fff;
    height: 43rem;
}

input, textarea, select, button, button, ul li {
    color:#112233;
    font-style: normal;
    font-weight: bold;
    line-height: normal;
    font-size: 16px;
}

.bg-blue {
    background:#44CCFF;
    color:#fff;
    border:none;
}

.bg-darkblue {
    background:#112233;
    color:#fff;
    border:none;
}

.bg-none {
    background: none;
    border:none;
}

button {
    text-align: center;
    cursor:pointer;
}

.CTA-small {
    width:auto;
    padding: 10px;
    border-radius:5px;
}

.CTA-medium {
    padding: 16px;
    line-height: 20px;
    font-size: 20px;
    border-radius: 5px;
    width: 133px;
}

body {
    margin:0px;
}

@media screen and (max-width:800px) {
    .content {
    width:100%;
}

h1 {
    font-size: 29px;
}

h5 {
    line-height: 28px;
    font-size: 13px;
}
}

@media screen and (max-width: 1000px) {
    h1 {
    line-height: 30px;
    font-size: 23px;
    }
}
@media screen and (min-width:2000px) {
    .header, .content {
    width:100% !important;
    padding-right: 13.3% !important;
    padding-left: 13.3% !important;
}
}


</style>