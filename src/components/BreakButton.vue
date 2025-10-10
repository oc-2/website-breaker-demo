<template>
   <div class="break-button" @click="destroy" >
     Break Me
   </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import breakWebPage from "@oc-2/website-breaker";
import "../assets/BreakButton.css";

export default defineComponent({
  name: "page-destroyer",
  props: {
    msg: String,
  },

  methods: {
    destroy(){
      breakWebPage();
    }
  }
});
</script>
