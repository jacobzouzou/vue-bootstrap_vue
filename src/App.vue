<template>
  <!--Collapse module-->
  <div id="app" class="container">
    <br />
    <h1>Use "bootstrap-vue" package</h1>
    <br />
    <p>
      <b-btn v-b-toggle.collapse1 variant="warning">Toggle Collapse</b-btn>
    </p>
    <b-collapse id="collapse1">
      <b-card>
        Collapse contents Here
        <b-btn v-b-toggle.collapse2 size="sm">Toggle Inner Collapse</b-btn>
        <b-collapse id="collapse2" class="mt-2">
          <b-card>Hello!</b-card>
        </b-collapse>
      </b-card>
    </b-collapse>
    <!--rows-->
    <b-row class="border">
      <b-col cols="12" md="8">cols="12"</b-col>
    </b-row>
    <b-row class="border">
      <b-col cols="12" mt="8">cols="12"</b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style lang="scss">
@import "./assets/custom.scss";
@import "../node_modules/bootstrap/scss/bootstrap.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.border {
  border: solid black thin;
}
</style>
