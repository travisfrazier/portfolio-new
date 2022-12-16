<template>
  <Layout>
    <Header />
    <Skills />
    <Projects />
    <Contact />
    <Rings class="header__rings" />
    <Rings class="skills__rings" />
    <Rings class="footer__rings" />
  </Layout>
</template>


<script>
import Header from '../components/Header.vue';
import Skills from '../components/Skills.vue';
import Projects from '../components/Projects.vue';
import Contact from '../components/Contact.vue';
import Rings from '../components/Rings.vue';



export default {
  metaInfo: {
    title: 'Travis Frazier'
  },
  components: {
    Header,
    Skills,
    Projects,
    Contact,
    Rings
  },
  methods: {
    animateSkills() {
      //One
      gsap.set('.skills__rings .one', {
        x: 100
      })
      gsap.to(".skills__rings .one", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.skills__rings'
      });

      //Two
      gsap.set('.skills__rings .two', {
        x: 125
      })
      gsap.to(".skills__rings .two", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.skills__rings'
      });

      //Three
      gsap.set('.skills__rings .three', {
        x: 150
      })
      gsap.to(".skills__rings .three", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.skills__rings'
      });

      //Four
      gsap.set('.skills__rings .four', {
        x: 175
      })
      gsap.to(".skills__rings .four", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.skills__rings'
      });

      //Five
      gsap.set('.skills__rings .five', {
        x: 200
      })
      gsap.to(".skills__rings .five", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.skills__rings'
      });
    },
    animateHeader() {
      //One
      gsap.set('.header__rings .one', {
        x: -100
      })
      gsap.to(".header__rings .one", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
      });

      //Two
      gsap.set('.header__rings .two', {
        x: -125
      })
      gsap.to(".header__rings .two", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
      });

      //Three
      gsap.set('.header__rings .three', {
        x: -150
      })
      gsap.to(".header__rings .three", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
      });

      //Four
      gsap.set('.header__rings .four', {
        x: -175
      })
      gsap.to(".header__rings .four", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
      });

      //Five
      gsap.set('.header__rings .five', {
        x: -200
      })
      gsap.to(".header__rings .five", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
      });
    },
    animateFooter() {
      //One
      gsap.set('.footer__rings .one', {
        x: -100
      })
      gsap.to(".footer__rings .one", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.footer__rings'
      });

      //Two
      gsap.set('.footer__rings .two', {
        x: -125
      })
      gsap.to(".footer__rings .two", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.footer__rings'
      });

      //Three
      gsap.set('.footer__rings .three', {
        x: -150
      })
      gsap.to(".footer__rings .three", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.footer__rings'
      });

      //Four
      gsap.set('.footer__rings .four', {
        x: -175
      })
      gsap.to(".footer__rings .four", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.footer__rings'
      });

      //Five
      gsap.set('.footer__rings .five', {
        x: -200
      })
      gsap.to(".footer__rings .five", {
        duration: 2,
        x: 0,
        repeat: 0,
        yoyo: true,
        scrollTrigger: '.footer__rings'
      });
    },
  },
  mounted() {
    this.animateSkills();
    this.animateHeader();
    this.animateFooter();
  }
}
</script>

<style lang="scss" scoped>
.home-links a {
  margin-right: 1rem;
}

.skills__rings {
  position: absolute;
  right: -250px;
  top: 1050px;
  @media only screen and (max-width: $mobile) {
    right: -350px;
    top: 1450px;
  }
}

.header__rings {
  position: absolute;
  left: -150px;
  top: 120px;
  @media only screen and (max-width: $mobile) {
      left: -350px;
  }
}

.footer__rings {
  position: absolute;
  bottom: 190px;
  left: -150px;
  @media only screen and (max-width: $mobile) {
    left: -350px;
    bottom: 180px;
  }
}
</style>
