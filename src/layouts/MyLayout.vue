<template>
  <q-layout view="hhh lpr fff">
    <q-header elevated reveal>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          @click="leftDrawerOpen = !leftDrawerOpen"
          icon="fas fa-bars"
          aria-label="Menu"
        />

        <q-toolbar-title>
          Rafael E. Ferrero
        </q-toolbar-title>

      </q-toolbar>
    </q-header>

    <q-footer elevated>
      <div><small>Powered by </small>Quasar v{{ $q.version }}</div>
    </q-footer>

    <q-drawer
      v-model="leftDrawerOpen"
      bordered
      content-class="bg-grey-2"
      side="left"
      behavior="mobile"
      overlay
    >
      <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px;">
        <q-list>
          <q-item clickable tag="a" target="_blank" href="https://www.linkedin.com/in/rafaeleferrero">
            <q-item-section avatar>
              <q-icon name="fas fa-book" />
            </q-item-section>
            <q-item-section>
              <q-item-label>Lea mi Blog</q-item-label>
              <!-- <q-item-label caption>@rafaeleferrero</q-item-label> -->
            </q-item-section>
          </q-item>
          <q-item clickable tag="a" target="_blank" href="https://www.linkedin.com/in/rafaeleferrero">
            <q-item-section avatar>
              <q-icon name="fas fa-at" />
            </q-item-section>
            <q-item-section>
              <q-item-label>Escríbame</q-item-label>
              <!-- <q-item-label caption>@rafaeleferrero</q-item-label> -->
            </q-item-section>
          </q-item>
        </q-list>
      </q-scroll-area>

      <q-img class="absolute-top bg-primary center" style="height: 150px">
        <div class="absolute-center text-center bg-transparent">
          <q-avatar size="90px" class="q-mb-sm">
            <img src="~assets/me.jpg">
          </q-avatar>
          <div class="text-weight-bold">Rafael E. Ferrero</div>
        </div>
      </q-img>

    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MyLayout',

  data () {
    return {
      leftDrawerOpen: false
    }
  }
}
</script>
