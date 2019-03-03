<template>
<div class="header-container">
  <header class="the-header">
    <TheSideNavToggle @toggle="$emit('sidenavToggle')" />
      <nuxt-link to="/"><img class="logo" /></nuxt-link>
    <div class="spacer"></div>
    <div class="navigation-items">
      <ul class="nav-list">
        <li class="nav-item">          
          <div class="dropdown">
            <button class="dropbtn navigation--listitems">For bedrifter</button>
            <div class="dropdown-content">
              <nuxt-link class="navigation--listitems" to="/24so1">24so1</nuxt-link>
              <nuxt-link class="navigation--listitems" to="/24so1">24so1</nuxt-link>
              <nuxt-link class="navigation--listitems" to="/24so1">24so1</nuxt-link>
            </div>
          </div>
          </li>
        <li class="nav-item">
          <div class="dropdown">
            <button class="dropbtn navigation--listitems">For regnskapsfører</button>
            <div class="dropdown-content">
              <nuxt-link class="navigation--listitems" to="/24so1">24so2</nuxt-link>
              <nuxt-link class="navigation--listitems" to="/24so1">24so2</nuxt-link>
              <nuxt-link class="navigation--listitems" to="/24so1">24so2</nuxt-link>
            </div>
          </div>
        </li>
        <li class="nav-item"><nuxt-link class="navigation--listitems" to="/Priser">Priser</nuxt-link></li>
      </ul>
    </div>
    <div class="header-buttons">
      <button class="CTA-small bg-none">Login</button>
      <button class="CTA-small bg-blue" style="margin-right:2rem;">Prøv Gratis</button>
    </div>
  </header>
</div>
</template>

<script>

import TheSideNavToggle from "@/components/Navigation/TheSideNavToggle";

export default {
  name: "TheHeader",
  components: {
    TheSideNavToggle
  }
};

</script>


<style scoped>
.dropbtn:after {
    font-family: FontAwesome;
    content: "\f000";
    font-family: Font Awesome 5 Pro;
    padding-left:1rem;
    color: #112233;
}
.navigation--listitems {
    font-family: Roboto;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
    font-size: 16px !important;
    color: #112233;
    padding: 10px !important;
    line-height: 1rem;
    background:transparent;
}

.dropbtn {
  padding: 16px;
  font-size: 16px;
  border: none;
}
.dropdown {
  position: relative;
  display: inline-block;
}
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #fff;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
  padding: 1rem 0rem 1rem 1rem;
}
.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}
.dropdown-content a:hover {background-color: #44CCFF;color:#fff;}
.dropdown:hover .dropdown-content {display: block;}
.dropdown:hover .dropbtn {color: #44CCFF;}

.header-logo {
  width:20%;
}

.header-buttons {
  width:30%;
}

.nav-items {
width: 50%;
}

.header-buttons .CTA-small {
  float:right;
}

.logo {
  height: 20px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url('~assets/images/logo.svg');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  min-width: 180px;
}

.header {
 /* width: 90%; 
  width:100%;*/
  display:flex;
  justify-content: center;
  align-items: center;
  padding-right: 5%;
  padding-left: 5%;
  margin-bottom:2rem;
}

.nav-items {
  list-style: none;
  padding: 0;
  margin:0;
  display:flex;
  justify-content: space-around;
  align-items: center;
}

ul li a {
  color:#282828;
  font-weight: 500;
  text-decoration:none;
}

@media screen and (max-width: 950px) {
  .header-logo, .logo {
    width:100%;
  }
  .header {
    display:table;
  }
  .header-buttons {
    display:none;
  }
}

@media screen and (min-width: 637px) and (max-width: 767px) {
  .header-buttons {
    display:table;
    width:40%;
  }
}

.header-container {
  height: 60px;
}

.the-header {
  width: 100%;
  position: fixed;
  height: 60px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  z-index: 100;
  box-sizing: border-box;
  padding: 0 14%;
  background:#fff;
}

.logo {
  margin: 0 10px;
  font-size: 1.3rem;
}

.logo a {
  text-decoration: none;
  color: white;
}

.spacer {
  flex: 1;
}

.navigation-items {
  display: none;
}

@media (min-width: 768px) {
  .navigation-items {
    display: block;
  }
}

@media (min-width:768px) and (max-width:1270px) {
  .the-header {
    padding: 0 1%;
  }
}

.nav-list {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}

.nav-item {
  margin: 0 10px;
}

.nav-item a {
  text-decoration: none;
}

.nav-item a:hover,
.nav-item a:active,
.nav-item a.nuxt-link-active {
  color: #44CCFF;
}


.nav-item .dropdown-content a:hover {
  color: #fff !important;
}

.dropdown-content a {
  padding: 2rem auto;
}
</style>
