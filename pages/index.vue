<template>
  <div>
    <h1>{{ title }}</h1>
    <p>This is the home page.</p>
    <my-component />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import MyComponent from '~/components/MyComponent.vue';

@Component({
  components: {
    MyComponent,
  },
})
export default class IndexPage extends Vue {
  title: string = 'Welcome to My SPA Nuxt App!';
}
</script>

