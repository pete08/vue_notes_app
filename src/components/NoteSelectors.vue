<template>
  <div class="note-selectors">
    <note-selector /> 
    <note-selector /> <note-selector /> 
    <div class="note-selector">
      <p class="note-selector-title">Second note...</p>
      <p class="note-selector-timestamp">Timestamp here...</p>
    </div>
    <div class="note-selector">
      <p class="note-selector-title">Third note...</p>
      <p class="note-selector-timestamp">Timestamp here...</p>
    </div>
  </div>
</template>


<script>
import NoteSelector from "./NoteSelector";

export default {
  name: "note-selectors",
  components: {
    NoteSelector    
  }
};
</script>