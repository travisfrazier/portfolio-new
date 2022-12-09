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
    title: 'Hello, world!'
  },
  components: {
    Header,
    Skills,
    Projects,
    Contact,
    Rings
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
