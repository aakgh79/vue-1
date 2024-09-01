<template>
  <div id="ProjectsView" style="width: 100%; height:100%vh; background-color: yellow">
    <div class="row">
      <div class="col-3">
        <strong class="d-flex justify-content-evenly"
          ><h1>projects >>></h1></strong
        >
      </div>
    </div>

    <ToDoList></ToDoList>
  </div>
</template>



<script>
import ToDoList from "@/components/ToDoList.vue";

export default {
  components: { ToDoList },
  data() {
    return {};
  },
  mounted() {},

  methods: {},
};
</script>