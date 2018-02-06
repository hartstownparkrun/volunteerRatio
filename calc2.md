## Calulate your run to volunteer ratio below
<div id="div1">
<p id="p1">.</p>

</div>

<script>
var para = document.createElement("p");
var node = document.createTextNode("This is new. 2");
para.appendChild(node);
var element = document.getElementById("div1");
element.appendChild(para);
  function myFunction() {
    document.getElementById("p1").innerHTML = "Button clicked";
}
</script>

<div>
  <div><span># of runs</span><span><input></span><br>
  <div><span># of volunteering</span><span><input></span>
</div>
    <button onclick="myFunction()">Calculate</button>
