<template lang="html">
  <div class="container center-align">

  <div class="row">
    <h1>ROI calculator </h1>
<div class="row container">

  <graph class="col s12"/>

</div>


    <form>
      <div class="row">

        <div class="column">
        <div class="input-field col s4">
          <select>
            <option value="0" disabled selected required>Required</option>
            <option value="1">1-4</option>
            <option value="2">5-10</option>
            <option value="3">10-25</option>
            <option value="4">25+</option>
          </select>
          <label>Number of employees</label>
        </div>
      </div>

        <div class="column">
        <div class="input-field col s4">
          <select>
            <option value="0" disabled selected required>Required</option>
            <option value="1">Solidworks</option>
            <option value="2">Pro/E</option>
            <option value="3">Creo</option>
            <option value="4">NX</option>
          </select>
          <label>Your current CAD system</label>
        </div>
      </div>

      <div class="column">
      <div class="input-field col s4">
        <select>
          <option value="0" disabled selected required>Required</option>
          <option value="1">Standard</option>
          <option value="2">Professional</option>
          <option value="3">Premium</option>
        </select>
        <label>Current packages</label>
      </div>
    </div>



      </div>

            <div>


              <form action="#">
                <h3><label>packages</label></h3>
                <p>

                  <label>
                    <input type="checkbox" />
                    <span>FEA</span>
                  </label>
                  <div/>

                  <label>
                    <input type="checkbox" />
                    <span>CFD</span>
                  </label>

                  <label>
                    <input type="checkbox" />
                    <span>Routing</span>
                  </label>
                </p>
              </form>




            </div>



      <div class="row">
        <div class="input-field col s4">
          <textarea id="textarea2" class="materialize-textarea" data-length="120"></textarea>
          <label for="textarea2">Describe the problem</label>
        </div>
      </div>



    <button class="btn waves-effect waves-light blue darken-2" type="submit">Request a quote
  <i class="material-icons right">send</i>
</button>
    </form>

</div>

</div>
</template>

<script>


import graph from "./graph"

export default {

  name: 'roi',
  components: {
    graph
  },
  data () {
    return {
      msg: 'Welcome to Onshape print'
    }
  }
}


document.addEventListener('DOMContentLoaded', function() {
   var elems = document.querySelectorAll('select');
   var options = document.querySelectorAll('option');
   var instances = M.FormSelect.init(elems, options);})




</script>

<style>
/* div.container {
    width: 70%;
    min-width: 350px;
} */


</style>
