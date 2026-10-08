# estiliza-o-de-formulario-css

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog - Inscrição</title>

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f0f2f5;
            margin: 0;
            padding: 30px 16px;
            color: #333;
        }

        header {
            text-align: center;
            margin-bottom: 30px;
        }

        main {
            max-width: 800px;
            margin: 0 auto;
        }

        .form-container {
            max-width: 600px;
            margin: 0 auto;
            padding: 30px;
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
        }

        .form-container h2 {
            margin-top: 0;
            color: #2c3e50;
        }

        .form-row {
            display: flex;
            justify-content: space-between;
            gap: 20px;
        }

        .form-group {
            display: flex;
            flex-direction: column;
            gap: 8px;
            flex: 1;
            margin-bottom: 18px;
        }

        label {
            font-size: 14px;
            font-weight: bold;
        }

        input,
        select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 6px;
            font-size: 16px;
            background-color: #fff;
        }

        input:focus,
        select:focus {
            outline: 2px solid #3498db;
            outline-offset: 1px;
        }

        button {
            width: 100%;
            padding: 14px;
            background-color: #3498db;
            color: #ffffff;
            border: none;
            border-radius: 6px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #2176ae;
        }

        footer {
            text-align: center;
            margin-top: 25px;
            font-size: 14px;
            color: #666;
        }

        @media (max-width: 500px) {
            .form-row {
                flex-direction: column;
                gap: 0;
            }

            .form-container {
                padding: 20px;
            }
        }
    </style>
</head>

<body>
    <header>
        <h1>Meu Blog</h1>
        <p>Inscreva-se para receber nossas novidades!</p>
    </header>

    <main>
        <section class="form-container">
            <h2>Formulário de inscrição</h2>

            <form action="#" method="post">
                <div class="form-row">
                    <div class="form-group">
                        <label for="nome">Nome completo:</label>
                        <input
                            type="text"
                            id="nome"
                            name="nome"
                            placeholder="Digite seu nome"
                            autocomplete="name"
                            required
                        >
                    </div>

                    <div class="form-group">
                        <label for="email">E-mail:</label>
                        <input
                            type="email"
                            id="email"
                            name="email"
                            placeholder="seu@email.com"
                            autocomplete="email"
                            required
                        >
                    </div>
                </div>

                <div class="form-group">
                    <label for="categoria">Categoria de interesse:</label>
                    <select id="categoria" name="categoria" required>
                        <option value="">Selecione uma categoria</option>
                        <option value="tecnologia">Tecnologia</option>
                        <option value="design">Design</option>
                        <option value="programacao">Programação</option>
                        <option value="outros">Outros</option>
                    </select>
                </div>

                <button type="submit">Inscrever-se</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; Bungas 2026</p>
    </footer>
</body>
</html>
```
