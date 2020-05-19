
<template>
  <q-layout view="lHh lpR lFf">

    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="left = !left" />

        <q-toolbar-title>
          Team Rocket Project
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer show-if-above v-model="left" side="left" elevated>
      <q-list padding class="q-mt-sm">
            <q-item active clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="storage" />
              </q-item-section>

              <q-item-section>
              Insert Data
              </q-item-section>
            </q-item>

            <q-item  clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="bar_chart" />
              </q-item-section>

              <q-item-section>
              Look at data
              </q-item-section>
            </q-item>
          </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
export default {
  data () {
    return {
      left: false
    }
  }
}
</script>
<style lang="scss" scoped>
</style>