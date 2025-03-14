<!DOCTYPE html>
<html>
<head>
<title>Calculadora Basica</title>
<style>
input[id="Tela"] {
width: 200px;
height: 30px;
}
input[type="button"] {
width: 50px;
height: 30px;
}
</style>
</head>
<body>
<h2>Calculadora Basica</h2>
<input id="Tela" type="text" readonly>
<br>
<br>
<input type="button" value="C" onclick="limpar()">
<input type="button" value=""  onclick="append('')">
<input type="button" value=""  onclick="append('')">
<input type="button" value="/" onclick="append('/')">
<br>
<input type="button" value="1" onclick="append('1')">
<input type="button" value="2" onclick="append('2')">
<input type="button" value="3" onclick="append('3')">
<input type="button" value="*" onclick="append('*')">
<br>
<input type="button" value="4" onclick="append('4')">
<input type="button" value="5" onclick="append('5')">
<input type="button" value="6" onclick="append('6')">
<input type="button" value="-" onclick="append('-')">
<br>
<input type="button" value="7" onclick="append('7')">
<input type="button" value="8" onclick="append('8')">
<input type="button" value="9" onclick="append('9')">
<input type="button" value="+" onclick="append('+')">
<br>
<input type="button" value="0" onclick="append('0')">
<input type="button" value="." onclick="append('.')">
<input type="button" value=""  onclick="append('')">
<input type="button" value="=" onclick="calcular()">


<script>

function calcular() {
let visor = document.getElementById('Tela').value;
let resultado = eval(visor);
document.getElementById('Tela').value = resultado;
}

function append(value) {
document.getElementById('Tela').value += value;
}

function limpar() {
document.getElementById('Tela').value = '';
}

</script>

</body>
</html>