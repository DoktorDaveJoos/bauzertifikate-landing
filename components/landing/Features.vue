<script setup>

import {
  File,
  Hammer,
  Earth,
  Building,
  Calculator,
  Sparkles
} from 'lucide-vue-next';

const features = [
  {
    title: "Energieausweise",
    description:
        "Erhalten Sie detaillierte Energieausweise für Ihre Gebäude, um deren Energieeffizienz zu bewerten und Verbesserungspotenziale zu identifizieren.",
    icon: File,
  },
  {
    title: "Sanierungsfahrpläne",
    description:
        "Nutzen Sie unsere Sanierungsfahrpläne, um systematisch und effektiv Sanierungsmaßnahmen zu planen, fördern und umzusetzen, die die Energieeffizienz Ihrer Gebäude verbessern.",
    icon: Hammer,
  },
  {
    title: "QNG Zertifikate",
    description:
        "Profitieren Sie von unseren Qualitätsnachweisen für Gebäude (QNG), die Ihre Gebäudequalität und Nachhaltigkeit bescheinigen und Ihr Engagement für umweltfreundliche Praktiken unterstreichen.",
    icon: Earth,
  },
  {
    title: "Zentrale Gebäudeverwaltung",
    description:
        "Verwalten Sie all Ihre Gebäudezentralisiert und effizient über unsere Plattform, um Daten zu erfassen, Maßnahmen zu planen und die Energieeffizienz kontinuierlich zu optimieren.",
    icon: Building,
  },
  {
    title: "Förderrechner",
    description:
        "Nutzen Sie unsere Förderrechner, um schnell und einfach Fördermöglichkeiten von KfW und BAFA für Ihre Sanierungsprojekte zu ermitteln und finanzielle Unterstützung zu erhalten.",
    icon: Calculator,
  },
  {
    title: "Expose Generator",
    description:
        "Generieren Sie professionelle Exposés für Ihre Gebäude mit wenigen Klicks, um potenziellen Interessenten alle relevanten Informationen über Energieeffizienz und Nachhaltigkeit zur Verfügung zu stellen.",
    icon: Sparkles,
  },
];
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">
      Unsere Leistungen im Überblick
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      Entdecken Sie die vielseitigen Funktionen von bauzertifikate, die Ihnen helfen, Energieeffizienz zu maximieren und
      Ihre Gebäude nachhaltig zu verwalten. Erfahren Sie, wie unsere Plattform Ihnen dabei hilft, den Überblick zu
      behalten und kosteneffiziente Lösungen zu implementieren.
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="item of features" class="flex gap-4 items-start">
      <div class="bg-black flex items-center justify-center rounded-full p-2 w-8 h-8 shrink-0">
        <Component :is="item.icon" class="text-white"/>
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ item.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
