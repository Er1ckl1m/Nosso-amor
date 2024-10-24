# Nosso-amor
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nosso Amor - Erick & Luan</title>
    <style>
        body {
            background-color: #f0f8ff;
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 0;
        }
        header {
            background-color: #ff69b4;
            padding: 20px;
            color: white;
            font-size: 2.5em;
        }
        .subtitle {
            color: #ffb6c1;
            font-size: 1.5em;
        }
        .photo-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 30px;
        }
        .photo {
            width: 100px;
            height: 100px;
            margin: 10px;
            border-radius: 50%;
            background-size: cover;
            transition: all 0.3s ease;
        }
        .photo:hover {
            width: 180px;
            height: 180px;
            box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.2);
        }
        footer {
            background-color: #ff69b4;
            color: white;
            padding: 20px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

    <header>
        Nosso Amor, Erick & Luan
        <div class="subtitle">Desde 30 de Novembro de 2023</div>
    </header>

    <section class="photo-container" id="photoContainer">
        <!-- Fotos dinâmicas serão inseridas aqui -->
    </section>

    <footer>
        <p>Feliz 1 ano de amor, com carinho, Erick & Luan.</p>
    </footer>

    <script>
        // Array de imagens hospedadas no GitHub
        const images = [];
        for (let i = 1; i <= 26; i++) {
            images.push(`https://github.com/seu-usuario/seu-repositorio/raw/main/image${i}.jpg`);
        }

        // Seleciona o contêiner onde as imagens serão inseridas
        const photoContainer = document.getElementById('photoContainer');

        // Cria as divs com as fotos
        images.forEach((src) => {
            const photoDiv = document.createElement('div');
            photoDiv.classList.add('photo');
            photoDiv.style.backgroundImage = `url(${src})`;
            photoContainer.appendChild(photoDiv);
        });
    </script>
