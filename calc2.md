## Calulate your run to volunteer ratio below
<div id="div1">
<p id="p1">.</p>

</div>

<script>
  function myFunction() {
    var runs = document.getElementById("runs").value;
    var vols = document.getElementById("vols").value;
  
    document.getElementById("p1").innerHTML = runs + ":" + vols ;
}
</script>

<div>
  <div><span># of runs</span><span><input type="text" name="runs" id="runs" value="" /></span><br>
  <div><span># of volunteering</span><span><input type="text" name="vols" id="vols" value="" /></span>
</div>
    <button onclick="myFunction()">Calculate</button>
