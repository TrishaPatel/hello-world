<template>
  <div class="md-layout  md-alignment-center">
    <div class="md-layout-item md-size-40">
      <md-content>
        <md-field>
          <label>Enter Your name</label>
          <md-input v-model="userName"></md-input>
        </md-field>
        <h3 v-if="userName">Welcome! {{ userName }}</h3>
      </md-content>
    </div>
  </div>
</template>

<script>
export default {
  name: "UserWelcome",
  data() {
    return {
      userName: ""
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
  color: #42b983;
}
</style>
