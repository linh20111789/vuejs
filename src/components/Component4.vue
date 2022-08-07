<template>
  <div>
    <p> Component 4</p>
  </div>

  <h2>改善項目リスト</h2>
  <table id="table3" class="table-matrix table table-hover table-striped table-responsive">
      <thead id="table3header">
        <tr>
          <th> Header 1 </th>
          <th> Header 2 </th>
        </tr>
      </thead>    
      <tbody>
        <tr>
            <td>Ram</td>
            <td>21</td>
            <td>Male</td>
            <td>Doctor</td>
        </tr>
        <tr>
            <td>Mohan</td>
            <td>32</td>
            <td>Male</td>
            <td>Teacher</td>
        </tr>  
      </tbody>     

  </table>

</template>

<script>
export default {
  name: "Component-4",
  props: ['email'],
};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
