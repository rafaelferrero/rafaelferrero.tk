<template>
  <q-page class="flex flex-center">
    <img alt="Quasar logo" src="~assets/quasar-logo-full.svg">
        <q-page-sticky position="bottom-right" :offset="[18, 18]">
        <q-fab color="secondary" push icon="fas fa-user-tag" active-icon="fas fa-times" direction="left">
        <q-fab-action
          clickable
          tag="a"
          target="_blank"
          href="https://github.com/rafaelferrero"
          color="accent"
          icon="fab fa-github" />
        <q-fab-action
          clickable
          tag="a"
          target="_blank"
          href="https://www.linkedin.com/in/rafaeleferrero"
          color="accent"
          icon="fab fa-linkedin" />
        <q-fab-action
          clickable
          tag="a"
          target="_blank"
          href="https://www.instagram.com/rafaeleferrero/"
          color="accent"
          icon="fab fa-instagram" />
        <q-fab-action
          clickable
          tag="a"
          target="_blank"
          href="https://twitter.com/rafaeleferrero"
          color="accent"
          icon="fab fa-twitter" />
        <q-fab-action
          clickable
          tag="a"
          target="_blank"
          href="https://fb.me/rafaeleferrero"
          color="accent"
          icon="fab fa-facebook" />
        </q-fab>
        </q-page-sticky>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex'
}
</script>
