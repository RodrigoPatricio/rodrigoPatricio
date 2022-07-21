<template>
  <section class="showcase">
    <div class="social-medias">
      <a :href="linkedinLink">
        <img src="@/assets/icons/linkedin.png" alt="Linkedin" />
        <p class="white">Linkedin</p>
      </a>
      <a :href="githubLink">
        <img src="@/assets/icons/github.png" alt="GitHub" />
        <p class="white">GitHub</p>
      </a>
      <a :href="twitterLink">
        <img src="@/assets/icons/twitter.png" alt="Twitter" />
        <p class="white">Twitter</p>
      </a>
    </div>

    <div class="rodrigo">
      <h1>Rodrigo Patricio</h1>
      <h2>UI • UX • FRONT-END</h2>
      <a href="../documents/RodrigoPatricio.pdf" download="RodrigoPatricio.pdf"><button>Download Resume</button></a>
    </div>

    <img id="arrow" src="@/assets/icons/arrow.png" alt="arrow" />

    <div class="about">
      <h3>ABOUT ME</h3>
      <div class="line"></div>
      <p>
        I’m a software engineer<br />
        specialized in web and app development<br />
        focused on user experience.
      </p>
      <a href="https://wa.me/5513982000646"><button>Get in touch</button></a>
    </div>
  </section>

  <section class="tech">
    <div>
      <h5>UI / UX DESIGN</h5>
      <p>User Interface Design</p>
      <p>Interaction Design</p>
      <p>User Experience Thinking</p>
      <p>Prototyping</p>
      <p>Wireframing</p>
    </div>
    <div>
      <h5>FRONT-END</h5>
      <p>HTML5 / CSS3</p>
      <p>JQuery & JavaScript libraries</p>
      <p>Vue.js</p>
      <p>Responsive Design</p>
      <p>Sass</p>
      <p>Git</p>
    </div>
  </section>

  <div class="line-short"></div>

  <section class="works">
    <h5>MY WORKS</h5>
    <p>
      A Selection of recent projects I’ve been working on<br />landing pages,
      websites, apps...
    </p>
  </section>
  <Works />
  <div class="line-short"></div>

  <section class="contact">
    <h5>GET IN TOUCH</h5>
    <a href="mailto:rp.patricio@yahoo.com"
      ><button>rp.patricio@yahoo.com</button></a
    >
    <div class="social-medias">
      <a :href="linkedinLink">
        <img src="@/assets/icons/linkedin-red.png" alt="Linkedin" />
        <p class="red">Linkedin</p>
      </a>
      <a :href="githubLink">
        <img src="@/assets/icons/github-red.png" alt="GitHub" />
        <p class="red">GitHub</p>
      </a>
      <a :href="twitterLink">
        <img src="@/assets/icons/twitter-red.png" alt="Twitter" />
        <p class="red">Twitter</p>
      </a>
    </div>
  </section>
  <footer>
    <p class="white">© 2022 Rodrigo Patricio. All rights reserved.</p>
  </footer>
</template>

<script>
import Works from "@/components/Works.vue";
export default {
  components: {
    Works,
  },
  data() {
    return {
      linkedinLink: "https://linkedin.com/in/rodrigo-pinto-patricio",
      githubLink: "https://github.com/RodrigoPatricio",
      twitterLink: "https://twitter.com/rodrigoo_patt",
    };
  },
};
</script>

<style>
@import url("@/assets/base.css");
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Montserrat:wght@800&family=Ubuntu:wght@400;500;700&display=swap");
.showcase {
  background: url("@/assets/background.png") no-repeat;
  background-size: cover;
  background-position: center;
  min-height: 1143px;
  padding-top: 50px;
}
.social-medias,
.social-medias a {
  margin: 0 2.5% 0 2.5%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: nowrap;

  text-decoration: none;
}
.social-medias p {
  font-family: ubuntu;
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  /* identical to box height */

  margin: 0 6px 0 6px;
}

.about p {
  color: #ffffff;
}
.tech {
  margin: 200px 0 150px 0;
  background: white;
  color: black;
  display: flex;
  align-items: top;
  justify-content: space-around;
  flex-wrap: wrap;
}
.tech p {
  color: #888888;
}

.works p {
  color: #888888;
}

.contact {
  margin: 0 0 150px 0;
}
</style>
