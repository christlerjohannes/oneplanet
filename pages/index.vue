<template>
  <div id="page">
    <div class="header">
      <h1>ONE PLANET. ONE VISION</h1>

      <p class="">
        Eine prosperierende Zukunft für uns alle ist möglich – auch vor dem
        Hintergrund einer wachsenden Weltbevölkerung und einem erhöhten Bedarf
        an Ressourcen. Wir sind ONE PLANET, ein gemeinnütziges
        Umweltschutz-Start-up. Wir möchten informieren, inspirieren sowie
        Forschung anregen. <b>– ONE PLANET. ONE VISION</b>
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
        uns gegenübersehen. Untätigkeit ist keine Option.
      </p>

      <p>
        Daher haben wir uns zum Ziel gesetzt, mit führenden
        Klimawissenschaftlerinnen und Klimawissenschaftlern zu kooperieren. Um
        eine Informationsplattform zur
        <b>Veröffentlichung sämtlicher relevanten Klimadaten</b> zu schaffen.
        Als vertrauensvolle Grundlage für einen sachlich fundierten
        gesellschaftlichen Diskurs. Transparent und verständlich.
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
        <source src="~/static/schlieren2.mp4" type="video/mp4" />
      </video>

      <div class="content">
        <h2>Forschung und Entwicklung</h2>
      </div>
    </div>
      <div class="text-section">
        <p>
          Vor uns steht die größte zivilisatorische Transformation der
          Geschichte. Um diese gigantische Herausforderung zu meistern,
          benötigen wir eine Vielzahl von Ideen und Lösungen. Als nicht
          profitorientierte Organisation stehen uns
          <b>keine Interessenkonflikte</b> im Weg. Wir sind in der Lage,
          entkoppelt von jeglichen – ökonomischen wie politischen – Einflüssen
          oder Zwängen zu agieren. Um jene Technologien zu forcieren, die aus
          unserer Sicht die stärkste Kraft entfalten zur Gestaltung einer
          nachhaltigen Zukunft.
        </p>

        <p>
          So halten wir das friedliche Zusammenleben von 11 Milliarden Menschen
          für erreichbar. Mit einem Zeithorizont von 10.000 Jahren bei
          europäischem Lebensstandard – ohne dabei den Planeten an seine
          Belastungsgrenzen zu bringen. Es ist die Stunde der Wissenschaft, der
          Forschung, der Visionen und Taten.
        </p>

        <h3>ONE PLANET. ONE SPIRIT</h3>
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
        <h2>ONE PLANET. ONE MISSION.</h2>
      </div>
    </div>

    <div class="text-section">
      <p>
        ONE PLANET verfolgt als vordringliches Ziel, die weltweiten
        CO2-Emissionen von jährlich 38 Gigatonnen zu neutralisieren – und
        langfristig
        <b
          >den CO2-Gehalt der Atmosphäre auf ein vorindustrielles Niveau zu
          senken</b
        >. Das Non-Profit-Start-up setzt auf einen lebendigen Austausch; auf
        Kommunikation, Kooperation und Konnektivität.
      </p>

      <p>
        Die Geschichte zeigt, dass wir imstande sind, Herausragendes leisten.
        Mit der uns Menschen angeborenen Fähigkeit, innovativ und kreativ zu
        sein, Allianzen zu bilden, unsere Kräfte zu vereinen und zu bündeln,
        ausgerichtet auf ein Ziel: den Weg für eine nachhaltige Zukunft zu
        ebenen.
      </p>

      <h3>ONE PLANET. ONE MISSION</h3>
    </div>

    <!-- Context Form -->

    <form ref="form" @submit.prevent="sendEmail">
      <label>Name</label>
      <input type="text" name="user_name" />
      <label>Email</label>
      <input type="email" name="user_email" />
      <label>Message</label>
      <textarea name="message"></textarea>
      <input type="submit" value="Send" />
    </form>
  </div>
</template>


<script>
import emailjs from "@emailjs/browser";

export default {
  name: "oneplanet",

  methods: {
    sendEmail() {
      emailjs
        .sendForm(
          "service_u0emxmi",
          "template_mtj07ac",
          this.$refs.form,
          "CwHSxBgv6QMDgLyFA"
        )
        .then(
          (result) => {
            alert("Nachricht wurde gesendet!");
            this.$refs.form.reset();
          },
          (error) => {}
        );
    },
  },
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
  font-size: 72px;
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