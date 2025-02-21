<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simulador de Economia - Dellta Solar</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background: white;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
            border-radius: 8px;
        }
        h1 {
            color: #ff9900;
        }
        label {
            display: block;
            margin: 10px 0 5px;
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .btn {
            background: #ff9900;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        .btn:hover {
            background: #e68a00;
        }
        .result {
            display: none;
            margin-top: 20px;
            font-size: 18px;
            font-weight: bold;
            color: green;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Descubra Quanto Você Pode Economizar!</h1>
        <form id="simuladorForm">
            <label for="conta">Valor Médio da Conta de Luz (R$)</label>
            <input type="number" id="conta" required>
            
            <label for="tipo">Tipo de Imóvel</label>
            <select id="tipo" required>
                <option value="residencial">Residencial</option>
                <option value="comercial">Comercial</option>
                <option value="industrial">Industrial</option>
            </select>
            
            <label for="cidade">Cidade</label>
            <input type="text" id="cidade" required>
            
            <label for="nome">Seu Nome</label>
            <input type="text" id="nome" required>
            
            <label for="whatsapp">Seu WhatsApp</label>
            <input type="tel" id="whatsapp" required>
            
            <button type="button" class="btn" onclick="calcularEconomia()">Calcular Economia</button>
        </form>
        
        <div id="resultado" class="result"></div>
    </div>

    <script>
        function calcularEconomia() {
            var conta = parseFloat(document.getElementById('conta').value);
            if (!conta || conta <= 0) {
                alert('Por favor, insira um valor válido para a conta de luz.');
                return;
            }
            
            var economia = conta * 0.9; // Simulação de economia de 90%
            
            document.getElementById('resultado').innerHTML = 
                `Você pode economizar até <strong>R$ ${economia.toFixed(2)}</strong> por mês! 🚀`;
            document.getElementById('resultado').style.display = 'block';
        }
    </script>
</body>
</html>
