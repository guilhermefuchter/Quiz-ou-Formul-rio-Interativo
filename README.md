# Quiz-ou-Formul-rio-Interativo


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz Interativo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        h1 {
            text-align: center;
            margin-top: 30px;
            color: #333;
        }

        form {
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        label {
            display: block;
            margin-bottom: 10px;
            color: #333;
        }

        input[type="radio"] {
            margin-right: 10px;
        }

        button[type="submit"] {
            display: block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button[type="submit"]:hover {
            background-color: #0056b3;
        }

        #resultado {
            margin-top: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Quiz Interativo</h1>
    <form id="quizForm">
        <label for="q1">1. Qual é a capital do Brasil?</label><br>
        <input type="radio" id="q1a" name="q1" value="brasilia"> Brasília<br>
        <input type="radio" id="q1b" name="q1" value="rio"> Rio de Janeiro<br>
        <input type="radio" id="q1c" name="q1" value="sao_paulo"> São Paulo<br><br>

        <label for="q2">2. Qual é a cor do céu em um dia ensolarado?</label><br>
        <input type="radio" id="q2a" name="q2" value="azul"> Azul<br>
        <input type="radio" id="q2b" name="q2" value="verde"> Verde<br>
        <input type="radio" id="q2c" name="q2" value="amarelo"> Amarelo<br><br>

        <button type="submit">Enviar Respostas</button>
    </form>

    <div id="resultado"></div>

    <script>
        document.getElementById('quizForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Impede o envio padrão do formulário

            // Captura as respostas
            var resposta1 = document.querySelector('input[name="q1"]:checked');
            var resposta2 = document.querySelector('input[name="q2"]:checked');

            // Valida as respostas
            if (!resposta1 || !resposta2) {
                alert('Por favor, responda todas as perguntas.');
                return;
            }

            // Processa as respostas
            var pontuacao = 0;
            if (resposta1.value === 'brasilia') {
                pontuacao++;
            }
            if (resposta2.value === 'azul') {
                pontuacao++;
            }

            // Mostra o resultado
            var resultadoDiv = document.getElementById('resultado');
            resultadoDiv.innerHTML = 'Você acertou ' + pontuacao + ' de 2 perguntas.';
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz Interativo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        h1 {
            text-align: center;
            margin-top: 30px;
            color: #333;
        }

        form {
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        label {
            display: block;
            margin-bottom: 10px;
            color: #333;
        }

        input[type="radio"] {
            margin-right: 10px;
        }

        button[type="submit"] {
            display: block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button[type="submit"]:hover {
            background-color: #0056b3;
        }

        #resultado {
            margin-top: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Quiz Interativo</h1>
    <form id="quizForm">
        <label for="q1">1. Qual é a capital do Brasil?</label><br>
        <input type="radio" id="q1a" name="q1" value="brasilia"> Brasília<br>
        <input type="radio" id="q1b" name="q1" value="rio"> Rio de Janeiro<br>
        <input type="radio" id="q1c" name="q1" value="sao_paulo"> São Paulo<br><br>

        <label for="q2">2. Qual é a cor do céu em um dia ensolarado?</label><br>
        <input type="radio" id="q2a" name="q2" value="azul"> Azul<br>
        <input type="radio" id="q2b" name="q2" value="verde"> Verde<br>
        <input type="radio" id="q2c" name="q2" value="amarelo"> Amarelo<br><br>

        <button type="submit">Enviar Respostas</button>
    </form>

    <div id="resultado"></div>

    <script>
        document.getElementById('quizForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Impede o envio padrão do formulário

            // Captura as respostas
            var resposta1 = document.querySelector('input[name="q1"]:checked');
            var resposta2 = document.querySelector('input[name="q2"]:checked');

            // Valida as respostas
            if (!resposta1 || !resposta2) {
                alert('Por favor, responda todas as perguntas.');
                return;
            }

            // Processa as respostas
            var pontuacao = 0;
            if (resposta1.value === 'brasilia') {
                pontuacao++;
            }
            if (resposta2.value === 'azul') {
                pontuacao++;
            }

            // Mostra o resultado
            var resultadoDiv = document.getElementById('resultado');
            resultadoDiv.innerHTML = 'Você acertou ' + pontuacao + ' de 2 perguntas.';
        });
    </script>
</body>
</html>
