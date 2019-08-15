<template>
 <div id="app">
   <toolbar />
   <noteContainer />
 </div>
</template>
<script>
import Toolbar from "./components/Toolbar.vue";
import NoteContainer from "./components/NoteContainer.vue";
export default {
  name: 'app',
  components: {
    Toolbar,
    NoteContainer
  }
};
</script>

<style>
/* RESET */
* {
 margin: 0;
 padding: 0;
 border: 0;
 outline: none;
 box-sizing: border-box;
}

/* LAYOUT */
#app {
 display: flex;
 flex-direction: column;
 min-height: 100vh;
}
/* COLORS */
* {
 color: #454545;
 background-color: #FAFAF8;
}
/* TYPOGRAPHY */
body {
 font-family: sans-serif;
}

</style>