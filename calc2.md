<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js"></script>
## Calulate your run to volunteer ratio below
<style>
.error {
  color:red;
  }
.result{
  font-size:50px;
  }
</style>

<script>
  function updateError(element) {
     document.getElementById(element+"Error").innerHTML = "";
  }
  function myFunction() {
    var runs = document.getElementById("runs").value;
    var vols = document.getElementById("vols").value;  
    if(runs == null || runs==""){
      document.getElementById("runsError").innerHTML = "Please enter a value";}
    else {
     document.getElementById("runsError").innerHTML = "";}
    if(vols == null || vols==""){
      document.getElementById("volsError").innerHTML = "Please enter a value";}
    else{
      document.getElementById("volsError").innerHTML = "";}

    if (vols!="" && runs!=""){
      document.getElementById("p1").innerHTML = Math.round((runs/vols * 100) / 100) + ":1" ;}
    else {
      document.getElementById("p1").innerHTML = "";}
}
</script>

<div>
  <div><span># of runs</span><span><input onchange="updateError(this.name)" type="number" name="runs" id="runs" value="" /></span><span id="runsError" class="error"></span><br>
  <div><span># of volunteering</span><span><input onchange="updateError(this.name)" type="number" name="vols" id="vols" value="" /><span id="volsError" class="error"></span></span>
</div>
    <button onclick="myFunction()">Calculate</button>
    <p id="p1" class="result"></p>
