<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js"></script>
## Calulate your run to volunteer ratio below

# 15
<style>
.error {
  color:red;
  }
  
  .divTable
    {
        display:  table;
        width:auto;
        background-color:#eee;
        border:1px solid  #666666;
        border-spacing:5px;/*cellspacing:poor IE support for  this*/
       /* border-collapse:separate;*/
    }

    .divRow
    {
       display:table-row;
       width:auto;
    }

    .divCell
    {
        float:left;/*fix for  buggy browsers*/
        display:table-column;
        width:200px;
        background-color:#ccc;
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
      document.getElementById("p1").innerHTML = runs/vols + ":1" ;}
    else {
      document.getElementById("p1").innerHTML = "";}
}
</script>
    #of runs<input onchange="updateError(this.name)" type="number" name="runs" id="runs" value="" /><span id="runsError" class="error">
    #of volunteering<input onchange="updateError(this.name)" type="number" name="vols" id="vols" value="" /><span id="volsError" class="error">
	<button onclick="myFunction()">Calculate</button>
    
      <p id="p1"></p>
