<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Bootstrap3 Dialog Examples</h2>
    <ul>
      <li><a href="#" id="dialog0" onclick="BootstrapDialog.alert('I want banana!');" class="">BootstrapDialog Alert Demo</a></li><br>
      <li><a href="#" id="dialog1" onclick="BootstrapDialog.show({title: 'Say-hello dialog',message: 'Hi Apple!', type: BootstrapDialog.TYPE_WARNING, size: BootstrapDialog.SIZE_LARGE});" class="">BootstrapDialog Show Demo</a></li><br>
      <li><a href="#" id="dialog2" onclick="BootstrapDialog.alert({title: 'Loading message',message: $('<div></div>').load('/static/demo.html'), size: BootstrapDialog.SIZE_LARGE});" class="">BootstrapDialog Loading message from a file</a></li>
    </ul>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.min.css';
import 'bootstrap3-dialog/dist/css/bootstrap-dialog.min.css';

export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
