<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js"></script>
## Calulate your run to volunteer ratio below

# 3

<script>
  function myFunction() {
    var runs = document.getElementById("runs").value;
    var vols = document.getElementById("vols").value;
  
  console.log(runs);
  
  if(runs == null || runs==""){
    document.getElementById("p1").innerHTML = "Please enter a value
  }
  if(vols == null || vols==""){
    document.getElementById("volsError").innerHTML = "Please enter a value
  }
  
  if (vols!="" && runs!="")
  {
    document.getElementById("p1").innerHTML = runs/vols + ":1" ;
    }
    else
    {
    document.getElementById("p1").innerHTML = "";
    }
}
</script>

<div>
  <div><span># of runs</span><span><input type="number" name="runs" id="runs" value="" /></span><span id="runsError" class="error"></span><br>
  <div><span># of volunteering</span><span><input type="number" name="vols" id="vols" value="" /><span id="volsError" class="error"></span></span>
</div>
    <button onclick="myFunction()">Calculate</button>
    <p id="p1"></p>
