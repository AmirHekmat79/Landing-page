<template>
  <q-layout view="lHh lpr lFf" container style="height: 100vh" >
    <NavbarSection/>
   <BannerSection/>
   <AvatarSection/>
      <router-view />
    <OurWorkSection/>
    <PricingCards/>
    <ContactSection/>
    <MapSection/>
    <FooterSection/>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'

import NavbarSection from 'src/components/NavbarSection.vue';
import FooterSection from 'src/components/FooterSection.vue';
import BannerSection from 'src/components/BannerSection.vue';
import AvatarSection from 'src/components/AvatarSection.vue';
import MapSection from 'src/components/MapSection.vue';
import PricingCards from 'src/components/PricingCards.vue';
import OurWorkSection from 'src/components/OurWorkSection.vue';
import ContactSection from 'src/components/ContactSection.vue'
export default defineComponent({
  name: 'MainLayout',
  components: {
    NavbarSection ,
    FooterSection ,
    BannerSection ,
    AvatarSection ,
    PricingCards,
    OurWorkSection,
    MapSection,
    ContactSection
  },

})
</script>

<style>
*{
  padding: 0;
  margin: 0;
}
html { height: 100%; overflow:auto; }
body { height: 100%; }
</style>