<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Calculator</title>
</head>
<body>
    <input type="text" id="result" disabled />
    <div>
        <input type="button" value="1" onclick="dis('1')" />
        <input type="button" value="2" onclick="dis('2')" />
        <input type="button" value="+" onclick="dis('+')" />
        <input type="button" value="=" onclick="myFunction()" />
        <input type="button" value="C" onclick="clr()" />
    </div>

    <script>
        function dis(val) {
            document.getElementById("result").value += val;
        }

        function myFunction() {
            let x = document.getElementById("result").value;
            let y = eval(x);
            document.getElementById("result").value = y;
        }

        function clr() {
            document.getElementById("result").value = "";
        }
    </script>
</body>
</html>
