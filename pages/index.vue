<template>
  <div id="page">
    <div class="header">
      <h1>ONE PLANET</h1>

      <p class="bold">
        ONE PLANET, ONE VISION: Eine prosperierende Zukunft ist möglich – für
        uns alle. Auch vor dem Hintergrund wachsender Weltbevölkerung und
        steigendem Ressourcenbedarf.
      </p>

      <p>
        Indem wir anfangen, unsere Lebensbereiche emissionsfrei zu gestalten.
        Indem wir entschlossen neue Wege gehen. Konsequent in Richtung
        Kreislaufwirtschaft. Indem es uns als Weltgemeinschaft gelingt, die
        Erderwärmung aufzuhalten.
      </p>

      <p>
        Wir sind ONE PLANET, ein gemeinnütziges Umweltschutz-Start-up. Wir
        möchten informieren, inspirieren und Forschung anregen. Für effektive
        Lösungen zum Klimaschutz.
      </p>

      <p class="bold">
        Gemeinsam gegen den Klimawandel. Für eine nachhaltige Zukunft.
      </p>
    </div>

    <div class="video-wrapper">
      <video
        id="video1"
        class="video video-1"
        autoplay
        loop
        muted
        poster="https://assets.codepen.io/6093409/river.jpg"
      >
        <source src="~/static/schlieren1.mp4" type="video/mp4" />
      </video>

      <div class="content">
        <h2>Informationskampagne</h2>
      </div>
    </div>

    <div class="text-section">
      <p>
        Was können wir konkret tun? Wie lassen sich gemeinschaftlich Mittel und
        Wege finden, um die globale Erderwärmung aufzuhalten? Was wir brauchen,
        ist eine ganzheitliche Vorstellung davon, welcher Herausforderung wir
        uns gegenübersehen. Dass Untätigkeit keine Option ist.
      </p>

      <p>
        Daher haben wir uns zum Ziel gesetzt, mit führenden
        Klimawissenschaftlerinnen und Klimawissenschaftlern zu kooperieren. Mit
        Universitäten und Forschungsinstituten. Um eine Informationsplattform
        zur <b>Veröffentlichung sämtlicher relevanten Klimadaten</b> zu
        schaffen. Transparent, verständlich und verantwortungsvoll. Als
        vertrauensvolle Grundlage für einen sachlich fundierten, für uns alle
        nachvollziehbaren gesellschaftlichen Diskurs. Eine Aufklärungsplattform,
        an der wir unser kollektives Handeln ausrichten.
      </p>

      <h3>ONE PLANET, ONE SPIRIT.</h3>
    </div>

    <!-- NEXT SECTION -->
    <div class="video-wrapper">
      <video
        id="video1"
        class="video video-2"
        autoplay
        loop
        muted
        poster="https://assets.codepen.io/6093409/river.jpg"
      >
        <source src="~/static/schlieren2.mp4" type="video/mp4" />
      </video>

      <div class="content">
        <h2>Forschung und Entwicklung</h2>
      </div>
    </div>

    <div class="text-section">
      <p>
        Vor uns steht die größte zivilisatorische Transformation der Geschichte.
        Um diese gigantische Herausforderung zu meistern, benötigen wir eine
        Vielzahl von Ideen und Lösungen. Als nicht profitorientierte
        Organisation stehen uns keine Interessenkonflikte im Weg. Wir sind in
        der Lage, entkoppelt von jeglichen – ökonomischen wie politischen –
        Einflüssen oder Zwängen zu agieren. Um jene Technologien zu forcieren,
        die aus unserer Sicht den größten Impact zur Gestaltung einer
        nachhaltigen Zukunft haben.
      </p>

      <p>
        Auf diesem Hintergrund halten wir das friedliche Zusammenleben von 11
        Milliarden Menschen für erreichbar. Mit einem Zeithorizont von 10.000
        Jahren bei europäischem Lebensstandard. Ohne den Planeten an seine
        Belastungsgrenzen zu bringen. Indem wir Technologien etablieren, die
        eine klimaneutrale Produktion, ein emissionsfreies Leben ermöglichen.
        Zudem gilt es Wege zu finden, bereits emittiertes CO2 in das inaktive
        Kohlenstoffkreislauf-System einzuspeisen – und somit unschädlich zu
        machen.
      </p>

      <p class="bold">
        Es ist die Stunde der Wissenschaft, der Forschung, der Visionen und
        Taten.
      </p>
    </div>

     <!-- NEXT SECTION -->
    <div class="video-wrapper">
      <video
        id="video1"
        class="video video-2"
        autoplay
        loop
        muted
        poster="https://assets.codepen.io/6093409/river.jpg"
      >
        <source src="~/static/schlieren3.mp4" type="video/mp4" />
      </video>

      <div class="content">
        <h2>UNSER ZIEL</h2>
      </div>
    </div>

    <div class="text-section">
      <p>
       todo
      </p>

      <p>
       todo
      </p>

      <p class="bold">
        Es ist die Stunde der Wissenschaft, der Forschung, der Visionen und
        Taten.
      </p>
    </div>

    <!-- Context Form -->

    <p>
        KONTAKT FORM
    </p>

  </div>
</template>

<script>
export default {
  name: "oneplanet",
};
</script>

<style lang="scss">
@font-face {
  font-family: Joschua_Gumpert_Schriftart;
  src: url("static/font.otf") format("opentype");
}

html,
body,
#__nuxt,
#__layout {
  height: 100% !important;
  width: 100% !important;
  padding: 0;
  margin: 0;
  max-width: 100%;
}

h2 {
  text-transform: uppercase;
}

.text-section {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

#page {
  // background: #f3f3f6;
  min-height: 100%;
  max-width: 100%;
}

p {
  max-width: 90%;
  max-width: 620px;
  padding: 16px;
  margin: 16px 0;
  text-align: center;

  &.bold {
    font-weight: bold;
  }
}

.header {
  min-height: 100vh;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.header-text {
  display: flex;
  align-items: center;
}

.video-wrapepr {
  margin-top: 1000px;
}

h1 {
  font-family: Joschua_Gumpert_Schriftart;
  font-size: 92px;
  font-weight: bold;
  color: #0c1122;
  margin: 32px 0;
}

.video-wrapper {
  position: relative;
}

.video {
  height: 150px;
  width: 100%;
  object-fit: cover;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: -1;
}

h3 {
  font-size: 32;
  font-weight: bold;
  margin-bottom: 32px;
}

.content {
  top: 0;
  position: absolute;
  z-index: 100;
  height: 150px;
  width: 100%;
  justify-content: center;
  align-items: center;
  vertical-align: middle;
}

h2 {
  font-family: Joschua_Gumpert_Schriftart;
  font-size: 48px;
  text-align: center;
  font-weight: bold;
  color: white;
  vertical-align: middle;
  line-height: 150px;
}
</style>