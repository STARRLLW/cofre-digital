# cofre-digital 
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário de Contato</title>
</head>
<body>
    <h2>Formulário de Contato</h2>
    <form action="#" method="post">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required><br><br>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required><br><br>

        <label for="mensagem">Mensagem:</label><br>
        <textarea id="mensagem" name="mensagem" rows="4" cols="30" required></textarea><br><br>

        <label for="data">Data:</label><br>
        <input type = "date"> 
        <button type="submit">Enviar</button>
    </form>
    <script>
        document.querySelector('form').addEventListener('submit', (e) => {
        const email = document.getElementById('email').value;
        if (!email.includes('@')) {
            alert('Email inválido!');
            e.preventDefault();
        }
    });
    </script>
</body>
</html>
