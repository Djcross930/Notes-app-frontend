

<script>
import NoteToolbar from './components/NoteToolbar'
import NoteContainer from './components/NoteContainer'
export default {
  components: {
    NoteToolbar,
    NoteContainer,
    NoteContainer
  }
}
</script>

<template>
  <div id="app">
    <NoteToolbar />
    <NoteContainer />
  </div>
</template>

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

.toolbar {
  padding: 0.5em;
}

.toolbar-button,
.toolbar-search {
  padding: inherit;
  border-radius: 0.3em;
}

.toolbar-search {
  float: right;
}

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
* {
  color: #454545;
  background-color: #FAFAF8;
}

.toolbar {
  background-color: #DCDADC;
}

.toolbar-button {
  background-color: #FFFFFF;
}

.toolbar-button:active {
  background-color: #AAAAAA;
}

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
body {
  font-family: sans-serif;
}

.note-selector-title {
  font-weight: bold;
}

.note-selector-timestamp {
  font-size: 0.7em;
}

.note-editor,
.note-editor-input {
  font-size: 0.9em;
}
</style>