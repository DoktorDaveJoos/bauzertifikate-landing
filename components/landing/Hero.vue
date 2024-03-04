<template>
  <main class="grid lg:grid-cols-2 place-items-center h-full pt-16 pb-8 md:pt-8">
    <div class="p-24 md:order-1 hidden md:block">
      <img
          class="rounded-full transition-transform transform hover:scale-125"
          src="~/assets/img/daniel-mccullough-unsplash.jpg"
          alt="Starship starts the engine"
          loading="eager"
          format="jpg"
          width="512"
          height="512"
      />
    </div>

    <div>
      <h1 class="text-4xl lg:text-5xl xl:text-6xl font-bold lg:tracking-tight">
        Energieberatung der Zukunft - Digital, Effizient, Transparent.
      </h1>
      <p class="text-lg mt-4 text-slate-600 max-w-xl">
        Bei bauzertifikate.de revolutionieren wir die Energieberatung durch Digitalisierung. Unsere Plattform ermöglicht die effiziente Erfassung und Verwaltung von Gebäudedaten, um nachhaltige Lösungen zu entwickeln. Willkommen in der Zukunft der Gebäudeeffizienz!
      </p>
      <div class="mt-6 flex flex-col sm:flex-row gap-3">
        <LandingLink
            style-name="primary"
            href="https://github.com/Gr33nW33n/nuxtship-template"
            target="_blank"
            rel="noopener"
        >Jetzt Demo anfragen
        </LandingLink
        >
        <LandingLink
            size="lg"
            styleName="outline"
            rel="noopener"
            href="https://github.com/Gr33nW33n/nuxtship-template"
            target="_blank"
        >View Repo
        </LandingLink
        >
      </div>
    </div>
  </main>
</template>
