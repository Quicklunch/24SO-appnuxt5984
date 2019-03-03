<template>
  <div class="badge-background">
    <div style="width:40%;" class="badge-contentbox">
      <div class="badge--textbox">
        <h1 style="text-align:left;margin-bottom: 0px;">Priser for Bedrifter</h1>
        <h5 style="margin-top: 0.5rem;">
          <strong>Din bedrift betaler per bruker per måned.
            <br>Forutsigbart og enkelt
          </strong>
        </h5>
        <span>Alle selskaper må minimum ha en «Start»-bruker, som også er brukeradmin. Detetter kan du velge pakker og enkeltmoduler - og knytte disse til ansatte i selskapet. Mobilversjonen av systemet følger brukerens tilganger på desktop.</span>
      </div>
    </div>
    <div style="width:60%;" class="badge-contentbox badge-graphicBG">
      <div class="badge-boxshadow">
        <h2>24SevenOffice Start</h2>
        <div style="float:left;width:100%;">
          <span class="badge--price">649,-</span>
          <span class="badge--pricetext">per måned
            <br>fakturert årlig
          </span>
        </div>
        <ul>
          <li>Regnskap</li>
          <li>Prosjektstyring</li>
          <li>CRM</li>
          <li>Faktura og ordre</li>
          <li>Timeregistrering</li>
          <li>Godkjenning</li>
          <li>Reiseregning og kjørebok</li>
        </ul>
        <div>
          <button class="CTA-medium bg-blue" style="float:left;">Prøv gratis</button>
          <button style="float:right;" class="CTA-medium bg-darkblue">Få tilbud</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scope>
.badge-boxshadow ul {
  list-style: none;
}

.badge-boxshadow ul li:before {
  content: "✓";
  color: rgba(68, 85, 102, 0.25);
  margin-right: 1rem;
}

.badge--textbox {
  width: 68%;
  margin: 0 auto;
}

.badge-boxshadow ul {
  margin: 2rem 0;
  float: left;
  width: 100%;
}

ul li {
  line-height: 30px;
}

.badge--pricetext {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  line-height: 24px;
  font-size: 16px;
  color: #2299ff;
  text-align: left;
  float: left;
  width: 45%;
  padding-top: 3%;
  padding-left: 5%;
}

.badge--price {
  font-style: normal;
  font-weight: normal;
  line-height: normal;
  font-size: 48px;
  text-align: right;
  color: #2299ff;
  float: left;
  width: 50%;
}

.badge-boxshadow {
  background: #ffffff;
  box-shadow: 0px 5px 14px rgba(0, 0, 0, 0.1);
  border-radius: 3px;
  padding: 30px;
  max-width: 35rem;
  min-width: 34rem;
  margin: 0 auto;
  display: table;
}
.badge-background {
  width: 100%;
  float: left;
  height: auto;
  background: #fff;
}

.badge-contentbox {
  float: left;
  width: 40%;
}

.badge-graphicBG {
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url("~assets/images/elements-graphic.svg");
  box-sizing: border-box;
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  /*height: -webkit-fill-available;
  width: 100%;*/
}

@media screen and (max-width: 800px) {
  .badge-contentbox {
    width: 100% !important;
    padding: 0px;
  }

  .badge--textbox {
    width: 95%;
  }
}
</style>