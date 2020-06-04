<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <section>
      Separate components

        <button-component buttonText="Example button"></button-component>
        <other-button-component buttonText="Other button"></other-button-component>

    </section>
    <section>
      Nested components
      <button-group-component></button-group-component>
    </section>
  </div>
</template>

<script>
import ButtonComponent from '../components/ButtonComponent';
import OtherButtonComponent from '../components/OtherButtonComponent';
import ButtonGroupComponent from '../components/ButtonGroupComponent';

export default {
  name: 'HelloWorld',
  components: {
    ButtonComponent,
    OtherButtonComponent,
    ButtonGroupComponent
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
section p{
  text-align: center;
}
</style>

