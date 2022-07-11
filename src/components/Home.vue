<template>
  <div class="home">
    <div class="card">
      <img alt="Headshot" src="../assets/me.jpg" />
      <h1>Hi, I'm {{ name }}!</h1>
      <p>
        I'm a computer science student at the University of Waterloo. I love
        learning about technology, travelling, and trying new things.
      </p>
      <p>
        Currently: looking for 2023 SWE/PM internships and planning my next
        hiking trip.
      </p>
      <p>Feel free to reach out for a quick chat or for my resume!</p>
      <ul>
        <a
          href="mailto:b55zhu@uwaterloo.ca"
          target="_blank"
          rel="noopener"
          class="icon"
        >
          <font-awesome-icon :icon="['far', 'envelope']" size="lg" />
        </a>
        <a
          href="https://github.com/bowenzhu1"
          target="_blank"
          rel="noopener"
          class="icon"
        >
          <font-awesome-icon :icon="['fab', 'github']" size="lg" />
        </a>
        <a
          href="https://linkedin.com/in/bowenzhu1"
          target="_blank"
          rel="noopener"
          class="icon"
        >
          <font-awesome-icon :icon="['fab', 'linkedin']" size="lg" />
        </a>
      </ul>
      <Footer />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Footer from "./Footer.vue";

@Options({
  components: {
    Footer,
  },
  props: {
    name: String,
  },
})
export default class Home extends Vue {
  name!: string;
}
</script>

<style scoped>
.card {
  margin: auto;
  background-color: rgb(255, 250, 245);
  border-radius: 16px;
  padding: 36px;
  max-width: 25rem;
  box-shadow: 0 15px 25px 0 rgba(0, 0, 0, 0.1);
}
img {
  border-radius: 50%;
  width: 14rem;
  height: 60%;
}
h3 {
  margin: 0 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
p {
  color: #7c7c7c;
  padding-bottom: 10px;
}
.icon {
  padding: 10px;
}
a {
  color: #000000;
}
</style>
