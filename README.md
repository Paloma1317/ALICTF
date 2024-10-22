# ALICTF

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de Premio</title>
</head>
<body>
    <h1>Introduce tu código para obtener un premio</h1>
    <form id="codigoForm">
        <input type="text" id="codigo" placeholder="Ingresa el código">
        <button type="button" onclick="verificarCodigo()">Enviar</button>
    </form>
    <p id="mensaje"></p>

    <script>
        function verificarCodigo() {
            var codigoIngresado = document.getElementById("codigo").value;
            var codigoCorrecto = "PREMIO123";  // Cambia esto al código que desees

            if (codigoIngresado === codigoCorrecto) {
                document.getElementById("mensaje").innerText = "¡Felicidades! Has ganado un premio.";
            } else {
                document.getElementById("mensaje").innerText = "Código incorrecto, intenta de nuevo.";
            }
        }
    </script>
</body>
</html>
