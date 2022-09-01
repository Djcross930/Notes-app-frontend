
<script>
import NoteSelector from './NoteSelector.vue';
import NoteEditor from './NoteEditor.vue'
export default {
  components: {
    NoteSelector,
    NoteSelector,
    NoteEditor
  }
}
</script>
<template>
  <div class="note-container">
    <NoteSelector />
    <NoteEditor />
  </div>
</template>