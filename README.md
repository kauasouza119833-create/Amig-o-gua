[xxxxprojeto.txt](https://github.com/user-attachments/files/24454588/xxxxprojeto.txt)
<!DOCTYPE html>
<html lang=“pt-br”>
<head>
  <meta charset=“UTF-8”>
  <title>Pedido de Gás</title>
</head>
<body>

  <h1>Pedido de Gás</h1>

  <form>
    <label>Nome:</label><br>
    <input type=“text” id=“nome”><br><br>

    <label>Endereço:</label><br>
    <input type=“text” id=“endereco”><br><br>

    <label>Tipo de Gás:</label><br>
    <select id=“gas”>
      <option>Gás 13kg</option>
      <option>Gás 45kg</option>
    </select><br><br>

    <button type=“button” onclick=“enviarPedido()”>Pedir Gás</button>
  </form>

  <script>
    function enviarPedido() {
      let nome = document.getElementById(“nome”).value;
      let endereco = document.getElementById(“endereco”).value;
      let gas = document.getElementById(“gas”).value;

      let mensagem = `Olá! Pedido de gás:%0A
Nome: ${nome}%0A
Endereço: ${endereco}%0A
Tipo: ${gas}`;

      window.open(`https://wa.me/5599999999999?text=${mensagem}`);
    }
  </script>

</body>
</html>
window.open
