<template>
  <div class="footer">
    <p>
      Made with Vue and ♥ by Bowen Zhu:
      <a
        href="https://github.com/bowenzhu1/bowenzhu1.github.io"
        target="_blank"
        rel="noopener"
      >
        source code
      </a>
    </p>
  </div>
</template>

<script lang="ts">
import { Vue } from "vue-class-component";

export default class Footer extends Vue {}
</script>

<style scoped>
.footer {
  align-self: flex-end;
  padding-top: 36px;
}
p {
  font-size: small;
  color: #7c7c7c;
}
a {
  color: #7c7c7c;
}
</style>
