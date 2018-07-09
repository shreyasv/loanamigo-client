<template>
  <div class="hello">

    <input type=text class='outline' placeholder='add to list' v-model="input"/>

    <button class='outline button' v-on:click="vals.push(input);input = ''">Add</button>

    <br><br>

    Text Count: {{input.length}}
    <ul>
      <div v-for="elem in vals"> {{elem}} </div></ul>


  </div>
</template>

<script>

function foo()  { console.log("hi")} // is this accessible?

export default {

  data: () => ({ input: "", vals: []  })

}

</script>

<style>

.outline {

  border: 1px solid #ccc;
  padding: 5px;

}

.button:hover {

  background-color: #f2f2f2;
}

</style>
