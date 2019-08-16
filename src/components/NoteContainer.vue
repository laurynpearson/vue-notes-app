<template>
  <div class="note-container">
     <note-selectors />
     <note-editor />
   </div>
</template>
<script>
import NoteSelectors from './NoteSelectors.vue';
import NoteEditor from './NoteEditor.vue';
export default {
  name: 'note-container',
  components: {
    NoteSelectors,
    NoteEditor
  }
};
</script>
<style>
/* LAYOUT */
.note-container {
 display: flex;
 flex: 1;
}
.note-selectors {
 flex: 0 0 13em;
}
.note-selector {
 padding: 1em;
}
.note-selector p {
 margin: 0;
}
.note-editor {
 display: flex;
 flex: 1;
 flex-direction: column;
}
.note-editor-info {
 padding: 0.5em;
 text-align: center;
}
.note-editor-input {
 display: flex;
 flex: 1;
 width: 100%;
 padding: 0 2em 0 2em;
}
/* COLORS */
.note-selectors {
 border-right: 1px solid #DCDADC;
}
.note-selector {
 border-bottom: 1px solid #DCDADC;
}
.note-selector.active {
 background-color: #FCE18D;
}
.note-selector-title {
 background-color: inherit;
}
.note-selector-timestamp {
 color: #626262;
 background-color: inherit;
}
.note-editor-info {
 color: #DCDADC;
}
/* TYPOGRAPHY */
.note-selector-title {
 font-weight: bold;
}
.note-selector-timestamp {
 font-size: 0.7em;
}
.note-editor, .note-editor-input {
 font-size: 0.9em;
}
</style>