<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MVT ARV/DEP Form</title>
</head>
<body>
    <h1>MVT ARV/DEP Bilgi Giriş Formu</h1>
    <form id="mvtForm">
        <label for="flt">FLT:</label><br>
        <input type="text" id="flt" name="flt"><br><br>

        <label for="reg">REG:</label><br>
        <input type="text" id="reg" name="reg"><br><br>

        <label for="sta">STA:</label><br>
        <input type="text" id="sta" name="sta"><br><br>

        <label for="std">STD:</label><br>
        <input type="text" id="std" name="std"><br><br>

        <label for="td">TD:</label><br>
        <input type="text" id="td" name="td"><br><br>

        <label for="dc">DC:</label><br>
        <input type="text" id="dc" name="dc"><br><br>

        <label for="ob">OB:</label><br>
        <input type="text" id="ob" name="ob"><br><br>

        <label for="pb">PB:</label><br>
        <input type="text" id="pb" name="pb"><br><br>

        <label for="dl">DL:</label><br>
        <input type="text" id="dl" name="dl"><br><br>

        <button type="button" onclick="generateMvtArv()">MVT ARV Oluştur</button>
        <button type="button" onclick="generateMvtDep()">MVT DEP Oluştur</button>
    </form>

    <script>
        function generateMvtArv() {
            var flt = document.getElementById("flt").value;
            var reg = document.getElementById("reg").value;
            var sta = document.getElementById("sta").value;
            var std = document.getElementById("std").value;
            var td = document.getElementById("td").value;
            var dc = document.getElementById("dc").value;
            var ob = document.getElementById("ob").value;
            var pb = document.getElementById("pb").value;
            var dl = document.getElementById("dl").value;

            var result = `MVT ARV - FLT: ${flt}, REG: ${reg}, STA: ${sta}, STD: ${std}, TD: ${td}, DC: ${dc}, OB: ${ob}, PB: ${pb}, DL: ${dl}`;
            alert(result);
        }

        function generateMvtDep() {
            var flt = document.getElementById("flt").value;
            var reg = document.getElementById("reg").value;
            var sta = document.getElementById("sta").value;
            var std = document.getElementById("std").value;
            var td = document.getElementById("td").value;
            var dc = document.getElementById("dc").value;
            var ob = document.getElementById("ob").value;
            var pb = document.getElementById("pb").value;
            var dl = document.getElementById("dl").value;

            var result = `MVT DEP - FLT: ${flt}, REG: ${reg}, STA: ${sta}, STD: ${std}, TD: ${td}, DC: ${dc}, OB: ${ob}, PB: ${pb}, DL: ${dl}`;
            alert(result);
        }
    </script>
</body>
</html>
