

<template>
  <div class="container mt-2" style="width: 100%; height: 200px; background-color: #a0ede3">
    <H1 style="text-align:center; color:blue; margin-top:0.25rem">To Do List</H1>
      
    <ul class="list-group">
      <li  type="text" class="list-group-item list-group-item-action" V-for="task in Todolist">{{ task }}</li>
    </ul>
    <p></p>
    <div>
      <input class="form-control" placeholder="type task" type="text" V-model="NewTask"/>
      <bottom @Click="AddTask" class="btn btn-warning">Add</bottom>
</div>


  </div>

</template>







<script>
// C.R.U.D
{
  // create
  // read
  // update
  // delete
}

export default {
  data() {
    return{
      Newtask:"",
      Todolist:["first task","second task"],
    };
  },

  mounted(){},

  methods:{
    AddTask(){
      if( this.NewTask.length>0){
        this.Todolist.push(this.NewTask)
        this.NewTask="";
      }
    },
      }

};
</script>