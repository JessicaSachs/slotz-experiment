<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <SearchForm>
      <slot><BaseButton slot="reference">BaseButton from App: Click me!</BaseButton></slot>
    </SearchForm>
  </div>
</template>

<script>
import { Vue, Component } from 'vue-property-decorator';
import SearchForm from './components/SearchForm';
import BaseButton from './components/BaseButton';

@Component({ components: { SearchForm, BaseButton }})
class App extends Vue {

}

export default App;

</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
