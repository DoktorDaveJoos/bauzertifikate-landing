<script setup>
import PartnerFeatures from "~/components/landing/PartnerFeatures.vue";

definePageMeta({
  layout: "landing",
});

const team = [
  {
    name: "Hannes Jungert",
    title: "Gründer, Energieberater & Ingenieur",
    avatar: {
      src: "/img/hannes_small.webp",
      width: 580,
      height: 580,
    },
  },
  {
    name: "David Joos",
    title: "Gründer & Softwareentwickler",
    avatar: {
      src: "/img/david_small.webp",
      width: 580,
      height: 580,
    },
  },


];
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>Partner werden</template>
      <template v-slot:desc>Profitieren Sie als Partner von bauzertifikate.de und gestalten Sie die Zukunft der
        Energieberatung mit.
      </template>
    </LandingSectionhead>

    <div class="flex justify-center gap-3 mx-auto max-w-4xl mt-10">
      <LandingLink href="/about" style-name="outline" size="md">Wer ist das?</LandingLink>
      <LandingLink href="/contact" size="md">Demo anfragen</LandingLink>
    </div>


      <PartnerFeatures></PartnerFeatures>


  </LandingContainer>
</template>
