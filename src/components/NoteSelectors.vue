<template>
  <div class="note-selectors">
    <note-selector 
      v-for="note in notes" 
      v-bind:key="note.id"
      v-bind:note="note"
    /> 

  </div>
</template>


<script>
import NoteSelector from "./NoteSelector";

export default {
  name: "note-selectors",

  components: {
    NoteSelector    
  },

  data: function() {
    return {
      notes: [
        { id: 1, body: "This is a first test", timestamp: Date.now() },
        { id: 2, body: "This is a second test", timestamp: Date.now() },
        { id: 3, body: "This is a third test", timestamp: Date.now() },
        { id: 4, body: "This is a fourth test", timestamp: Date.now() },
        { id: 5, body: "This is a fifth test", timestamp: Date.now() },
        { id: 6, body: "This is a sixth test", timestamp: Date.now() },
        { id: 7, body: "This is a seventh test", timestamp: Date.now() },
        { id: 8, body: "This is a eigth test", timestamp: Date.now() },
        { id: 9, body: "This is a ninth test", timestamp: Date.now() },
        { id: 10, body: "This is a tenth test", timestamp: Date.now() },
      ],
    };
  },
  

};

</script>