<script setup>
definePageMeta({
  layout: "landing",
});
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>Kontakt</template>
      <template v-slot:desc>Ob Partnerschaft, Kontakt oder sonstige Nachfragen.</template>
    </LandingSectionhead>

    <div class="grid md:grid-cols-2 gap-10 mx-auto max-w-4xl mt-16">
      <div>
        <h2 class="font-medium text-2xl text-gray-800">
          Kontaktieren Sie Uns.
        </h2>
        <p class="text-lg leading-relaxed text-slate-500 mt-3">
          Sie haben Fragen oder benötigen Unterstützung? Ob Partnerschaftsanfrage, Demoanfrage oder allgemeine Anfrage –
          wir sind für Sie da! Füllen Sie einfach das untenstehende Formular aus, und wir werden uns innerhalb von 48
          Stunden bei Ihnen melden, um Ihre Anliegen zu besprechen.
        </p>
        <div class="mt-5">
          <div class="flex items-center mt-2 space-x-2 text-gray-600">
            <Icon class="text-gray-400 w-4 h-4" name="uil:map-marker"/>
            <span>Marktstraße 41, Ravensburg</span>
          </div>
          <div class="flex items-center mt-2 space-x-2 text-gray-600">
            <Icon class="text-gray-400 w-4 h-4" name="uil:envelope"/>
            <a
                href="mailto:hannes@bauzertifikate.de"
            >hannes@bauzertifikate.de</a
            >
          </div>
          <div class="flex items-center mt-2 space-x-2 text-gray-600">
            <Icon class="text-gray-400 w-4 h-4" name="uil:envelope"/>
            <a
                href="mailto:david@bauzertifikate.de"
            >david@bauzertifikate.de</a
            >
          </div>
          <!-- <div class="flex items-center mt-2 space-x-2 text-gray-600">
            <Icon class="text-gray-400 w-4 h-4" name="uil:phone" /><a
              href="tel:+1 (234) 5678 999"
              >+1 (234) 5678 999</a
            >
          </div> -->
        </div>
      </div>
      <div>
        <LandingContactform/>
      </div>
    </div>
  </LandingContainer>
</template>
