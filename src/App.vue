<template>
  <div class="container">
    <div class="nav mb-3">
      <button>next</button>
      <button>prev</button>
    </div>

    <button-component v-if="indexPage === 1"></button-component>

    <circle-component v-else-if="indexPage === 2"></circle-component>

    <to-do-component v-else-if="indexPage === 3"></to-do-component>

    <form-component v-else></form-component>
  </div>
</template>

<script>
import ButtonComponent from "@/components/ButtonComponent";
import CircleComponent from "@/components/CircleComponent";
import ToDoComponent from "./components/ToDoComponent";
import FormComponent from "@/components/FormComponent";

export default {
  components: {
    ButtonComponent,
    CircleComponent,
    ToDoComponent,
    FormComponent,
  },
  data() {
    return {
      indexPage: 1,
    };
  },
};
</script>
