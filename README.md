# alura08
projeto para o alura 
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Henrique e Juliano - Acessibilidade</title>
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <header>
        <h1>Henrique e Juliano - Acessibilidade no Sertanejo</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#musicas">Músicas</a></li>
                <li><a href="#agenda">Agenda</a></li>
                <li><a href="#licencas">Licenças Creative Commons</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- Seção Home -->
        <section id="home">
            <h2>Bem-vindo ao site oficial de Henrique e Juliano!</h2>
            <p>Este site foi desenvolvido com o objetivo de divulgar o trabalho da dupla sertaneja de forma inclusiva e
                acessível a todos os públicos. Acompanhe as músicas, shows, notícias e muito mais.</p>
            <p>Estamos sempre em busca de novas formas de levar música e emoção para os nossos fãs!</p>
        </section>

        <!-- Seção Músicas -->
        <section id="musicas">
            <h2>Músicas</h2>
            <p>Confira as músicas mais populares de Henrique e Juliano. Clique no botão de play para ouvir as faixas diretamente
                no site!</p>

            <ul>
                <li>
                    <h3>Madri</h3>
                    <audio controls>
                        <source src="musicas/madri.mp3" type="audio/mp3">
                        Seu navegador não suporta o elemento de áudio.
                    </audio>
                </li>
                <li>
                    <h3>Flor e o Beija-Flor</h3>
                    <audio controls>
                        <source src="musicas/flor-beija-flor.mp3" type="audio/mp3">
                        Seu navegador não suporta o elemento de áudio.
                    </audio>
                </li>
                <li>
                    <h3>Cuida Bem Dela</h3>
                    <audio controls>
                        <source src="musicas/cuida-bem-dela.mp3" type="audio/mp3">
                        Seu navegador não suporta o elemento de áudio.
                    </audio>
                </li>
                <li>
                    <h3>Ex do Seu Atual</h3>
                    <audio controls>
                        <source src="musicas/ex-do-seu-atual.mp3" type="audio/mp3">
                        Seu navegador não suporta o elemento de áudio.
                    </audio>
                </li>
            </ul>
        </section>

        <!-- Seção Agenda -->
        <section id="agenda">
            <h2>Agenda de Shows</h2>
            <p>Confira a agenda de shows de Henrique e Juliano. Não perca a oportunidade de vê-los ao vivo!</p>

            <table>
                <thead>
                    <tr>
                        <th>Data</th>
                        <th>Local</th>
                        <th>Cidade</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>15/09/2025</td>
                        <td>Espaço de Shows</td>
                        <td>São Paulo - SP</td>
                    </tr>
                    <tr>
                        <td>20/09/2025</td>
                        <td>Arena Sertaneja</td>
                        <td>Rio de Janeiro - RJ</td>
                    </tr>
                    <tr>
                        <td>25/09/2025</td>
                        <td>Estádio Nacional</td>
                        <td>Brasília - DF</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <!-- Seção Licenças Creative Commons -->
        <section id="licencas">
            <h2>Licenças Creative Commons</h2>
            <p>Todo o conteúdo deste site, incluindo músicas, imagens e textos, segue as licenças Creative Commons, permitindo
                o compartilhamento e a adaptação de forma responsável. A licença CC permite que você compartilhe e remixe nosso conteúdo
                com as devidas atribuições.</p>
            <p>Você pode usar o conteúdo disponível no site, mas lembre-se de dar créditos adequados e não usar de forma comercial, conforme
                a licença especificada.</p>
        </section>
    </main>

    <!-- Menu de Acessibilidade -->
    <div id="menu-acessibilidade" class="menu-acessibilidade">
        <button class="menu-toggle">🔧 Acessibilidade</button>
        <div class="opcoes">
            <button id="aumento-fonte">A+</button>
            <button id="diminuir-fonte">A-</button>
        </div>
    </div>

    <footer>
        <p>© 2025 Henrique e Juliano. Todos os direitos reservados. Licenciado sob Creative Commons.</p>
    </footer>

    <script src="scripts.js"></script>
</body>

</html>
/* Reset básico de estilos */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    font-size: 16px; /* Tamanho de fonte inicial */
    transition: font-size 0.3s ease;
    padding: 0 20px;
    color: #333;
}

header {
    background-color: #f8f8f8;
    padding: 20px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

header h1 {
    color: #4CAF50;
}

nav ul {
    list-style-type: none;
    padding: 10px;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #333;
}

h1, h2, h3 {
    font-size: 1.8em;
    margin-bottom: 10px;
}

h3 {
    font-size: 1.5em;
}

ul {
    padding-left: 20px;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #f8f8f8;
    margin-top: 40px;
    border-top: 2px solid #eaeaea;
}

footer p {
    font-size: 14px;
    color: #777;
}

/* Estilo das tabelas da agenda */
table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 20px;
}

th, td {
    padding: 10px;
    text-align: center;
    border: 1px solid #ddd;
}

th {
    background-color: #4CAF50;
    color: white;
}

/* Menu de acessibilidade */
#menu-acessibilidade {
    position: fixed;
    top: 10px;
    right: 10px;
    background-color: #000;
    color: #fff;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
}

#menu-acessibilidade .menu-toggle {
    background-color: #4CAF50;
    border: none;
    color: white;
    padding: 10px;
    cursor: pointer;
    font-size: 16px;
    border-radius: 5px;
}

#menu-acessibilidade .opcoes {
    display: none;
    margin-top: 10px;
}

#menu-acessibilidade .opcoes button {
    background-color: #ff9800;
    border: none;
    color: white;
    padding: 10px;
    margin: 5px;
    cursor: pointer;
    border-radius: 5px;
}

#menu-acessibilidade .menu-toggle.active + .opcoes {
    display: block;
}

audio {
    width: 100%;
    max-width: 500px;
    margin-top: 10px;
}
    let tamanhoFonte = 16; // Tamanho inicial da fonte

    // Aumentar fonte
    aumentoFonteBtn.addEventListener('click', function () {
        tamanhoFonte += 2;
        document.body.style.fontSize = tamanhoFonte + 'px';
    });

    // Diminuir fonte
    diminuirFonteBtn.addEventListener('click', function () {
        if (tamanhoFonte > 10) { // limite mínimo
            tamanhoFonte -= 2;
            document.body.style.fontSize = tamanhoFonte + 'px';
        }
    });

    // Mostrar/esconder menu de acessibilidade
    menuToggle.addEventListener('click', function () {
        menuToggle.classList.toggle('active');
        opcoesMenu.classList.toggle('active');
    });
});

