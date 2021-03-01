<template>
  <div class="main">
    <nav
      class="navbar fixed-top px-1"
      v-bind:class="[darkMode ? navbarDark : navbarLight]"
    >
      <div class="container-fluid">
        <a class="navbar-brand" href="#" style="font-weight: 700"
          >@rodnavarroc</a
        >
        <button
          v-on:click="
            darkMode = !darkMode;
            if (darkMode) btnText = 'Lights On';
            if (!darkMode) btnText = 'Lights Off';
          "
          class="btn-sm"
          v-bind:class="[darkMode ? btnDark : btnLight]"
        >
          {{ btnText }}
        </button>
      </div>
    </nav>

    <div v-bind:class="[darkMode ? 'bg-dark text-light' : 'text-dark']">
      <div
        class="container px-4"
        style="width: 100%; height: 94vh; padding-top: 15vh"
      >
        <center>
          <img
            src="https://avataaars.io/?avatarStyle=Circle&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=BeardLight&facialHairColor=Black&clotheType=Hoodie&clotheColor=Blue03&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Smile&skinColor=Light"
          />
          <h1 style="font-weight: 700; font-size: 48px align-middle">
            <br />
            Hello! I'm glad you're here. 👋🏻
          </h1>
          <h4 class="text-muted" style="font-weight: 500">
            I'm Rodolfo, a software developer, graphic designer and mentor
            (sometimes).
          </h4>
          <br />

          <div class="d-none d-sm-block">
            <a
              href="https://github.com/rodnavarroc"
              class="link"
              target="_blank"
              rel="noopener"
              ><img
                src="https://img.icons8.com/bubbles/100/000000/github.png"
              />
            </a>

            <a
              href="https://linkedin.com/in/rodnavarroc"
              class="link"
              target="_blank"
              rel="noopener"
              ><img src="https://img.icons8.com/clouds/100/000000/linkedin.png"
            /></a>
            <br /><br />
          </div>

          <p>Read a little more about me scrolling down. 👇🏻</p>
        </center>
      </div>
      <br />
    </div>

    <div
      v-bind:class="[darkMode ? 'text-light' : 'text-dark']"
      v-bind:style="[
        darkMode ? { background: '#297185' } : { backgroundColor: '#c7ffff' },
      ]"
    >
      <div
        class="container px-4"
        style="
          width: 100%;
          height: auto;
          overflow: hidden;
          padding-top: 5vh;
        "
      >
        <div class="row">
          <div class="col-12">
            <h3>My (recent) Projects</h3>
            <p>
              Some of my work is listed here. All of them are source and free as always
              should be.
            </p>
            <br />
            <span></span>
          </div>
        </div>
        
      </div>
    </div>

    <div
      v-bind:class="[darkMode ? 'text-light' : 'text-dark']"
      v-bind:style="[
        darkMode ? { background: '#0a4545' } : { backgroundColor: '#8be8da' },
      ]"
    >
      <div
        class="container px-4"
        style="
          width: 100%;
          height: auto;
          overflow: hidden;
          padding-top: 5vh;
        "
      >
        <div class="row">
          <div class="col-12">
            <h3>My skills</h3>
            <p>I love doing cool stuff and learning a bit everyday.</p>
            <br />
            <span></span>
          </div>
        </div>

        <div class="row" style="font-size: 24px">
          <div class="col-12 col-md-6 pb-2" style="font-weight: 500">
            Web Development
          </div>
          <div class="col-12 col-md-6">
            <div class="row">
              <div
                class="col py-3 px-4"
                style="border-radius: 8px; font-weight: 400"
              >
                <p>
                  <b>NodeJS</b> with Express, Axios, scrape-api, and some
                  others.
                </p>
                <p><b>VueJS</b> in a middle level</p>
                <p><b>ReactJS</b> in a middle level</p>
              </div>
            </div>
          </div>
        </div>

        <div class="row" style="font-size: 24px">
          <div class="col-12 col-md-6 pb-2" style="font-weight: 500">
            Mobile Development
          </div>
          <div class="col-12 col-md-6">
            <div class="row">
              <div
                class="col py-3 px-4"
                style="border-radius: 8px; font-weight: 400"
              >
                <p><b>NodeJS</b> with some libraries for mobile development</p>
                <p><b>Angular</b> to create Android apps</p>
                <p><b>Ionic 4</b> to use with Angular</p>
              </div>
            </div>
          </div>
        </div>

        <div class="row" style="font-size: 24px">
          <div class="col-12 col-md-6 pb-2" style="font-weight: 500">
            Graphic and UI / UX
          </div>
          <div class="col-12 col-md-6">
            <div class="row">
              <div
                class="col py-3 px-4"
                style="border-radius: 8px; font-weight: 400"
              >
                <p><b>Adobe XD</b> to make UI / UX designs</p>
                <p><b>Lunacy</b> is also a great UI tool</p>
                <p><b>Photoshop and Illustrator</b> to graphic design</p>
              </div>
            </div>
          </div>
        </div>

        <div class="row" style="font-size: 24px">
          <div class="col-12 col-md-6 pb-2" style="font-weight: 500">
            Other languages and tools
          </div>
          <div class="col-12 col-md-6">
            <div class="row">
              <div
                class="col py-3 px-4"
                style="border-radius: 8px; font-weight: 400"
              >
                <p><b>SQL</b> for databases</p>
                <p>
                  <b>Python</b> for data analysis, neural networks (numpy,
                  pandas, keras) and some simulations
                </p>
                <p><b>Visual Basic and C</b> for desktop development</p>
                <p><b>Camtasia Studio</b> for video editing</p>
                <p></p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      darkMode: false,
      navbarDark: "text-light bg-dark",
      navbarLight: "text-dark bg-light",
      btnDark: "btn btn-outline-light",
      btnLight: "btn btn-outline-dark",
      footerLight: "text-light bg-dark",
      footerDark: "text-dark bg-light",
      btnText: "Lights On",
    };
  },
  name: "Base",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
  font-family: "Rubik", sans-serif;
}

.navbar-brand {
  text-decoration: none;
  color: inherit;
}

p {
  font-size: 18px;
}

a {
  color: inherit;
}
</style>
