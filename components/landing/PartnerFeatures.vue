<script setup>

import {
  BadgeEuro,
  UserRoundSearch,
  TrendingUp,
  Cloud,
  Smile,
  Gem
} from 'lucide-vue-next';

const features = [
  {
    title: "Monatliche Rechnung",
    description:
        "Erhalten Sie Ihre Abrechnungen bequem und transparent jeden Monat.",
    icon: BadgeEuro,
  },
  {
    title: "Direkter Ansprechpartner",
    description:
        "Profitieren Sie von einem persönlichen Ansprechpartner für eine individuelle Betreuung.",
    icon: UserRoundSearch,
  },
  {
    title: "Voller Zugang zu allen Leistungen",
    description:
        "Nutzen Sie unsere umfassenden Leistungen inklusive problemloser Abwicklung.",
    icon: Gem,
  },
  {
    title: "Nutzung der Immobilienplattform",
    description:
        "Erhalten Sie Zugang zu unserer innovativen Immobilienplattform für eine effiziente Verwaltung Ihrer Gebäudedaten.",
    icon: Cloud,
  },
  {
    title: "Höhere Kundenzufriedenheit",
    description:
        "Steigern Sie die Zufriedenheit Ihrer Kunden durch unsere maßgeschneiderten Lösungen und erstklassigen Service.",
    icon: Smile,
  },
  {
    title: "Höhere Effizienz",
    description:
        "Optimieren Sie Ihre Arbeitsabläufe und steigern Sie Ihre Effizienz mit unseren intelligenten Tools und Technologien.",
    icon: TrendingUp,
  },
];
</script>

<template>


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
