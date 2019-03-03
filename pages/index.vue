<template>
  <section>
      <div class="container">
      <BadgePriceBox/>
      <FullHorizontalButtons/>
      </div>
      <h1>Get more out of 24SevenOffice with <br> Add-ons & Integrations</h1>
      <postbox
      id="payment"
      icon="https://www.houseofcontrol.no/wp-content/uploads/2016/02/HOC-ikon-hus-m%C3%B8rkbl%C3%A5-RGB.png"
      title ="Lønn"
      previewText="Vi tilbyr en meget fleksibel og enkel prismodell  mot regnskapsbyråer."
      footerText="priser er pr. måned"
      price="35,-"
      />
      <postbox
      id="savings"
      icon="https://www.houseofcontrol.no/wp-content/uploads/2016/02/HOC-ikon-hus-m%C3%B8rkbl%C3%A5-RGB.png"
      title ="Lagring"
      previewText="Vi tilbyr en meget fleksibel og enkel prismodell rettet mot regnskapsbyråer."
      footerText="priser er pr. account pr. måned"
      price="449,-"
      />
      <postbox
      id="phonesupport"
      icon="https://www.houseofcontrol.no/wp-content/uploads/2016/02/HOC-ikon-hus-m%C3%B8rkbl%C3%A5-RGB.png"
      title ="Telefonsupport"
      previewText="Vi tilbyr en meget fleksibel og enkel prismodell  mot regnskapsbyråer."
      footerText="priser er pr. måned"
      price="500,-"
      />
  </section>
</template>


<style>
</style>

<script>
import BadgePriceBox from '~/components/badge/BadgePriceBox.vue'
import FullHorizontalButtons from '~/components/buttons/FullHorizontalButtons.vue'
import postbox from '~/components/posts/postbox.vue'

export default {
    components: {
        BadgePriceBox,
        FullHorizontalButtons,
        postbox
    }
}
</script>