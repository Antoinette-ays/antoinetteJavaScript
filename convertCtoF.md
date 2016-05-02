
<!DOCTYPE html>
<html>
<body>
<! Convertion of Celsius to Fahrenheit !>

<h1>Convertion</h1>
<form action = "demo">
Celsius: &nbsp &nbsp &nbsp<input id="cel" onchange="con_Temp('C')"> <br><br>
Fahrenheit:  <input id="far" onkeyup="con_Temp('F')"> 
<br><br> <button type="reset" value="Reset">Clear</button>
</form>
<script>
function con_Temp(deg)
{
  if (deg == "C") {
        var F 	= document.getElementById("cel").value * 9 / 5 + 32;
        document.getElementById("far").value = Math.round(F);
    } else	{
        var C 	= (document.getElementById("far").value -32) * 5 / 9;
        document.getElementById("cel").value = Math.round(C);
    }
}
</script>

</body>
</html>
