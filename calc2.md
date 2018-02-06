<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js"></script>
## Calulate your run to volunteer ratio below




<script>
  function myFunction() {
    var runs = document.getElementById("runs").value;
    var vols = document.getElementById("vols").value;
  
  if(runs == null){
  alert('please eneter a run');}
  
    document.getElementById("p1").innerHTML = runs/vols + ":1" ;
}
</script>

<div>
  <div><span># of runs</span><span><input type="number" name="runs" id="runs" value="" /></span><br>
  <div><span># of volunteering</span><span><input type="number" name="vols" id="vols" value="" /></span>
</div>
    <button onclick="myFunction()">Calculate</button>
    <p id="p1"></p>
