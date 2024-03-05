<script setup>
definePageMeta({
  layout: "landing",
});

const TeamImg3 = "https://source.unsplash.com/ZHvM3XIOHoE";

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
      <template v-slot:title>Über Uns</template>
      <template v-slot:desc>Wir sind ein leidenschaftliches Team aus Energieberatern und Softwareentwicklern.
      </template>
    </LandingSectionhead>

    <div class="flex flex-col gap-3 mx-auto max-w-4xl mt-16">
      <h2 class="font-bold text-3xl text-gray-800">
        Pioniere der Energieberatung.
      </h2>
      <p class="text-lg leading-relaxed text-slate-500">
        Unser Team ist angetreten, um die Energieberatung in eine aufregende neue Ära zu führen. Mit innovativen Ansätzen und einem fokussierten Blick auf die Zukunft gestalten wir die Branche neu. Unsere Leidenschaft für Nachhaltigkeit treibt uns an, während wir mit unserer technologischen Expertise bahnbrechende Lösungen entwickeln. Gemeinsam streben wir danach, die Energieberatung effizienter, intelligenter und umweltfreundlicher zu gestalten. Willkommen bei bauzertifikate.de – wo Innovation auf Energie trifft.
      </p>
    </div>
    <div class="grid md:grid-cols-2 gap-10 mx-auto max-w-4xl mt-12">
      <div v-for="item of team" class="group">
        <div class="w-full aspect-auto">
          <img
              :src="item.avatar.src"
              alt="Team"
              class="object-cover object-top rounded transition group-hover:-translate-y-1 group-hover:shadow-xl"
          />
        </div>

        <div class="mt-4 text-center">
          <h2 class="text-lg text-gray-800">{{ item.name }}</h2>
          <h3 class="text-sm text-slate-500">{{ item.title }}</h3>
        </div>
      </div>
      <!-- {
        team.map((item) => (
          <div class="group">
            <div class="w-full aspect-square">
              <Image
                {...item.avatar}
                format="avif"
                alt="Team"
                class="w-full h-full object-cover rounded transition  group-hover:-translate-y-1 group-hover:shadow-xl"
              />
            </div>

            <div class="mt-4 text-center">
              <h2 class="text-lg text-gray-800"> {item.name}</h2>
              <h3 class="text-sm text-slate-500"> {item.title}</h3>
            </div>
          </div>
        ))
      } -->
    </div>
  </LandingContainer>
</template>
