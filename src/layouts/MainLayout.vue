<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <img src="https://i.imgur.com/L5hnxTo.png" class="image-temp" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
    <div
      elevated
      class="
        full-width
        bg-white
        text-black
        q-pa-md
        row
        justify-evenly
        items-start
      "
    >
      <div class="col-3">
        <img src="https://i.imgur.com/L5hnxTo.png" class="image-temp" />
      </div>
      <div class="col-6 text-grey">
        ONEBID ASSET LLC, a company incorporated at Saint Vincent and the Grenadines with company number 2432 LLC 2022 with a registered address at unit Suite 305, Griffith Corporate Centre, Beachmont, Kingstown, Saint Vincent and the Grenadines. The company is regulated by the laws of Saint Vincent and the Grenadines and is fully capable and eligible to provide online Forex and CFDs trading services.<br><br>

The information on this website does not constitute investment advice or a recommendation or a solicitation to engage in any investment activity.<br><br>


Contacts:<br>

e-mail: <a href="mailto:info@onebidasset.com">info@onebidasset.com</a><br>

tel.: <a href="tel:+66811417611">+66811417611</a><br>
      </div>
    </div>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue';

const linksList = [
  {
    title: 'Docs',
    caption: 'quasar.dev',
    icon: 'school',
    link: 'https://quasar.dev',
  },
  {
    title: 'Github',
    caption: 'github.com/quasarframework',
    icon: 'code',
    link: 'https://github.com/quasarframework',
  },
  {
    title: 'Discord Chat Channel',
    caption: 'chat.quasar.dev',
    icon: 'chat',
    link: 'https://chat.quasar.dev',
  },
  {
    title: 'Forum',
    caption: 'forum.quasar.dev',
    icon: 'record_voice_over',
    link: 'https://forum.quasar.dev',
  },
  {
    title: 'Twitter',
    caption: '@quasarframework',
    icon: 'rss_feed',
    link: 'https://twitter.quasar.dev',
  },
  {
    title: 'Facebook',
    caption: '@QuasarFramework',
    icon: 'public',
    link: 'https://facebook.quasar.dev',
  },
  {
    title: 'Quasar Awesome',
    caption: 'Community Quasar projects',
    icon: 'favorite',
    link: 'https://awesome.quasar.dev',
  },
];

export default defineComponent({
  name: 'MainLayout',

  components: {},

  setup() {
    const leftDrawerOpen = ref(false);

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
});
</script>
