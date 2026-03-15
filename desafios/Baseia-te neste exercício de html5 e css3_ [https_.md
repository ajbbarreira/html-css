<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" style="height:64px;margin-right:32px"/>

# Baseia-te neste exercício de html5 e css3: [https://github.com/ajbbarreira/html-css/tree/main/desafios/d010](https://github.com/ajbbarreira/html-css/tree/main/desafios/d010) realizado pelos alunos do curso profissional de TIS.

Cria um exercício um pouco mais simples. Faz o enunciado e a solução.

Segue um exercício inspirado no d010 (Android), mas um pouco mais simples, adequado para TIS.

## Enunciado do exercício

Cria uma página chamada `desafio-simples.html` para apresentar um artigo sobre um **sistema operativo móvel** à tua escolha (Android, iOS, HarmonyOS, etc.).

A página deve cumprir estes requisitos:

1. Estrutura HTML

- Usar a declaração `<!DOCTYPE html>`.
- Definir idioma da página como português (`pt-PT`).

```
- Incluir `<meta charset="UTF-8">` e um `<title>` adequado.
```

2. Cabeçalho (header)

- Um `<header>` com fundo em degradé (duas tonalidades da mesma cor).
- Dentro do header:
    - Um `<h1>` com o título do site (ex.: “Tecnologia Mobile”).
    - Um `<p>` com uma pequena descrição (1–2 frases).

3. Navegação simples

- Logo abaixo do header, criar uma barra de navegação com um `<nav>`.
- Dentro do `<nav>`, colocar pelo menos 3 links (podem ser falsos com `href="#"`), por exemplo: “Início”, “Notícias”, “Contacto”.
- Aplicar estilo aos links: sem sublinhado, com cor clara, e efeito hover (mudar de cor ou sublinhar quando o rato passa por cima).

4. Conteúdo principal

- Usar um `<main>` para o conteúdo.
- Dentro do main, criar:
    - Um `<article>` com:
        - Um `<h2>` com o nome do sistema operativo escolhido.
        - Dois ou três parágrafos `<p>` com texto fictício sobre o sistema (história, características, etc.).

```
- Pelo menos um parágrafo deve ter algumas palavras em **negrito** e/ou *itálico* usando `<strong>` e `<em>`.
```


5. Imagem ilustrativa

- Inserir uma imagem relacionada com o sistema operativo (pode ser um logo genérico ou placeholder).
- A imagem deve ter:
    - `alt` descritivo.
    - Largura máxima de 300px aplicada via CSS, mantendo proporção.

6. Caixa de destaque (aside simples)

- Criar um `<aside>` com o título “Curiosidades”.
- Dentro do aside, colocar uma lista `<ul>` com 3 curiosidades (fictícias ou reais) sobre o sistema operativo.

7. Rodapé

- Criar um `<footer>` com:
    - Um parágrafo com o nome do autor (aluno) e o ano.
- Fundo diferente do resto da página e texto centrado.

8. Estilo geral (CSS em ficheiro externo)

- Criar um ficheiro `style.css` e ligá-lo no `<head>`.
- Requisitos mínimos de CSS:
    - Definir uma fonte sem serifa para o site.
    - Definir uma cor de fundo suave para o `<body>`.
    - Definir largura máxima para o `<main>` (por exemplo 800px) e centralizá-lo.

```
- Definir borda arredondada e sombra leve para o `<main>` ou `<article>`.
```

    - Garantir que a página fica legível em ecrãs pequenos (não precisa de media queries avançadas, apenas evitar larguras fixas exageradas).

Entrega:

- Ficheiro `desafio-simples.html`.
- Ficheiro `style.css`.
- Imagem usada (por exemplo na pasta `imagens/`).

***

## Possível solução (exemplo)

### Ficheiro `desafio-simples.html`

```html
<!DOCTYPE html>
<html lang="pt-PT">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tecnologia Mobile - Android</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tecnologia Mobile</h1>
        <p>Informação simples e clara sobre sistemas operativos móveis.</p>
    </header>

    <nav>
        <a href="#">Início</a>
        <a href="#">Notícias</a>
        <a href="#">Contacto</a>
    </nav>

    <main>
        <article>
            <h2>Android</h2>

            <p>
                O <strong>Android</strong> é um sistema operativo móvel baseado em Linux, 
                desenvolvido principalmente pela Google. É atualmente um dos sistemas 
                mais utilizados em smartphones e tablets em todo o mundo.
            </p>

            <p>
                Uma das grandes vantagens do Android é a sua <em>flexibilidade</em>. 
                Diversos fabricantes utilizam o sistema, criando uma enorme variedade 
                de dispositivos para diferentes necessidades e orçamentos.
            </p>

            <p>
                A loja oficial de aplicações do Android é a <strong>Google Play Store</strong>, 
                onde os utilizadores podem encontrar milhões de apps, jogos, livros e filmes.
            </p>

            <figure>
                <img src="imagens/android-logo.png" alt="Logótipo do sistema operativo Android">
                <figcaption>Exemplo de logótipo do Android.</figcaption>
            </figure>
        </article>

        <aside>
            <h3>Curiosidades</h3>
            <ul>
                <li>As primeiras versões do Android tinham nomes de doces.</li>
                <li>O Android foi inicialmente criado por uma pequena empresa em 2003.</li>
                <li>O sistema está presente também em TVs, relógios e carros.</li>
            </ul>
        </aside>
    </main>

    <footer>
        <p>Desenvolvido por [Nome do Aluno] &copy; 2026</p>
    </footer>
</body>
</html>
```


### Ficheiro `style.css`

```css
@charset "UTF-8";

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background-color: #e5f3ff;
    color: #222;
}

/* Cabeçalho com degradé */
header {
    background-image: linear-gradient(to right, #0059b3, #66a3ff);
    color: white;
    text-align: center;
    padding: 20px;
}

header h1 {
    margin-bottom: 10px;
}

/* Navegação simples */
nav {
    background-color: #003d80;
    padding: 10px;
    text-align: center;
}

nav a {
    color: #f0f8ff;
    text-decoration: none;
    margin: 0 10px;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
    color: #ffffff;
}

/* Conteúdo principal */
main {
    max-width: 800px;
    margin: 20px auto;
    padding: 15px;
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

article h2 {
    margin-bottom: 10px;
}

article p {
    margin-bottom: 10px;
    text-align: justify;
}

/* Imagem */
figure {
    text-align: center;
    margin: 15px 0;
}

figure img {
    max-width: 300px;
    width: 100%;
}

figure figcaption {
    font-size: 0.9em;
    color: #555;
}

/* Aside */
aside {
    background-color: #f0f7ff;
    border-left: 4px solid #0059b3;
    padding: 10px;
    margin-top: 15px;
    border-radius: 4px;
}

aside h3 {
    margin-bottom: 8px;
}

aside ul {
    list-style-type: square;
    margin-left: 20px;
}

/* Rodapé */
footer {
    background-color: #003359;
    color: white;
    text-align: center;
    padding: 10px;
    font-size: 0.9em;
}
```

Queres que eu adapte o enunciado para trabalhar também com um pequeno ficheiro `video.html` (como no desafio original, mas mais simples), ou preferes manter apenas uma página para já?
<span style="display:none">[^1_1][^1_10][^1_11][^1_12][^1_13][^1_14][^1_15][^1_2][^1_3][^1_4][^1_5][^1_6][^1_7][^1_8][^1_9]</span>

<div align="center">⁂</div>

[^1_1]: https://github.com/gustavoguanabara/html-css/blob/master/desafios/modulo-02/d010/desafio-android.pdf

[^1_2]: https://github.com/gustavoguanabara/html-css/issues/110

[^1_3]: https://github.com/backend-br/desafios

[^1_4]: https://github.com/OsProgramadores/op-desafios

[^1_5]: https://github.com/GabrielReira/Data-Science-Challenges

[^1_6]: https://www.youtube.com/watch?v=MnznvoNuy-I

[^1_7]: https://github.com/mgckaled/boracodar_desafios-rs

[^1_8]: https://www.youtube.com/watch?v=aO2yuiUEDgk

[^1_9]: https://github.com/eduardodaguinha/desafiosProjetoDIO

[^1_10]: https://cursos.alura.com.br/forum/topico-desafios-346262

[^1_11]: https://github.com/ocdigital/desafio-backend

[^1_12]: https://gustavoguanabara.github.io/html-css/

[^1_13]: https://github.com/rwurdig/Desafio-tecnico-engenharia-de-dados-Sicredi

[^1_14]: https://www.youtube.com/watch?v=Svnh2eaP4lE

[^1_15]: https://www.youtube.com/playlist?list=PLSo4Deley0aWeLCSCynh7PdrRCCc1gx2V


---

# Prefiro manter só uma página

Mantendo só uma página, o enunciado e a solução que te propus já estão completos e coerentes para um exercício ligeiramente mais simples que o d010 original.[^2_1]

Se quiseres, posso agora:

- Ajustar o nível (por exemplo, retirar `aside` ou `figure` para turmas mais fracas).
- Transformar este exercício numa ficha avaliativa com grelha de critérios (rubrica) pronta a usar.

Queres que prepare uma grelha de avaliação (com pesos para HTML, CSS, semântica, organização, etc.) para este exercício?

<div align="center">⁂</div>

[^2_1]: https://github.com/gustavoguanabara/html-css/blob/master/desafios/modulo-02/d010/desafio-android.pdf


---

# Adiciona uma área para um vídeo sobre plataformas de desenvolvimento para android e uma area para uma lista sobre a evolução histórica do android.

Segue uma versão atualizada do exercício com as duas novas áreas pedidas, mantendo tudo numa só página.

## Ajuste ao enunciado

Acrescentar aos requisitos anteriores:

9. Área para vídeo sobre plataformas de desenvolvimento Android
```
- Dentro do `<main>`, criar uma secção (pode ser um `<section>` ou `<div>`) com o título “Plataformas de desenvolvimento para Android”.
```

- Inserir um vídeo:
    - Pode ser um `<iframe>` incorporando um vídeo do YouTube sobre plataformas/IDE para Android (ex.: Android Studio, Flutter, etc.).[^3_1][^3_2]
    - Ou um `<video>` com ficheiro local (opcional).
- O vídeo deve estar centrado e ser responsivo: largura máxima 560px, ocupando 100% da largura disponível em ecrãs pequenos.[^3_3][^3_4]

10. Área para lista da evolução histórica do Android

- Ainda dentro do `<main>`, criar outra secção com o título “Evolução histórica do Android”.
- Adicionar uma lista ordenada `<ol>` com pelo menos 5 itens, cada um com:
    - Ano ou versão (ex.: “2008 – Android 1.0”).
    - Pequena descrição (1 frase) da importância dessa versão (primeiro lançamento, mudança de interface, etc.).[^3_5][^3_6][^3_7]

***

## Possível solução atualizada

### `desafio-simples.html` (com vídeo e lista histórica)

```html
<!DOCTYPE html>
<html lang="pt-PT">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tecnologia Mobile - Android</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tecnologia Mobile</h1>
        <p>Informação simples e clara sobre sistemas operativos móveis.</p>
    </header>

    <nav>
        <a href="#">Início</a>
        <a href="#">Notícias</a>
        <a href="#">Contacto</a>
    </nav>

    <main>
        <article>
            <h2>Android</h2>

            <p>
                O <strong>Android</strong> é um sistema operativo móvel baseado em Linux,
                desenvolvido principalmente pela Google. É atualmente um dos sistemas
                mais utilizados em smartphones e tablets em todo o mundo.
            </p>

            <p>
                Uma das grandes vantagens do Android é a sua <em>flexibilidade</em>.
                Diversos fabricantes utilizam o sistema, criando uma enorme variedade
                de dispositivos para diferentes necessidades e orçamentos.
            </p>

            <p>
                A loja oficial de aplicações do Android é a <strong>Google Play Store</strong>,
                onde os utilizadores podem encontrar milhões de apps, jogos, livros e filmes.
            </p>

            <figure>
                <img src="imagens/android-logo.png" alt="Logótipo do sistema operativo Android">
                <figcaption>Exemplo de logótipo do Android.</figcaption>
            </figure>
        </article>

        <aside>
            <h3>Curiosidades</h3>
            <ul>
                <li>As primeiras versões do Android tinham nomes de doces.</li>
                <li>O Android foi lançado comercialmente em 2008 com o HTC Dream.</li> <!-- [web:21][web:24][web:29] -->
                <li>Hoje está presente também em TVs, relógios e carros.</li>
            </ul>
        </aside>

        <section class="video-section">
            <h2>Plataformas de desenvolvimento para Android</h2>
            <p>
                Para desenvolver aplicações Android, é comum utilizar IDEs como
                <strong>Android Studio</strong> ou soluções multiplataforma como Flutter ou React Native.[web:22][web:27]
            </p>

            <div class="video-container">
                <!-- Substituir o src por um vídeo escolhido pelo aluno/professor -->
                <iframe
                    src="https://www.youtube.com/embed/l2UDgpLz20M"
                    title="Vídeo sobre desenvolvimento Android"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                    allowfullscreen>
                </iframe>
            </div>
        </section>

        <section class="history-section">
            <h2>Evolução histórica do Android</h2>
            <p>
                Abaixo está uma breve linha temporal com alguns marcos importantes na história do Android.[web:21][web:24][web:29]
            </p>
            <ol>
                <li><strong>2003</strong> – Criação da Android Inc., inicialmente focada em sistemas para dispositivos móveis.[web:21]</li>
                <li><strong>2005</strong> – Aquisição da Android Inc. pela Google.[web:21]</li>
                <li><strong>2008 – Android 1.0</strong> – Primeiro lançamento comercial no HTC Dream (T‑Mobile G1).[web:21][web:24][web:29]</li>
                <li><strong>2009 – Android 1.5 Cupcake</strong> – Início da tradição de nomes de doces para as versões.[web:29]</li>
                <li><strong>2011–2014</strong> – Consolidação do Android em vários fabricantes e crescimento global.[web:24][web:26]</li>
            </ol>
        </section>
    </main>

    <footer>
        <p>Desenvolvido por [Nome do Aluno] &copy; 2026</p>
    </footer>
</body>
</html>
```


### Ajustes adicionais em `style.css`

Acrescentar ao ficheiro anterior:

```css
/* Secção de vídeo */
.video-section {
    margin-top: 20px;
}

.video-section h2 {
    margin-bottom: 10px;
}

.video-section p {
    margin-bottom: 10px;
}

/* Contêiner responsivo para o iframe */
.video-container {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 */
    height: 0;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 0 8px rgba(0, 0, 0, 0.15);
    background-color: #000;
}

.video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

/* Secção de história */
.history-section {
    margin-top: 20px;
}

.history-section h2 {
    margin-bottom: 10px;
}

.history-section p {
    margin-bottom: 10px;
}

.history-section ol {
    margin-left: 20px;
}

.history-section li {
    margin-bottom: 6px;
}
```

Queres que eu agora transforme isto numa ficha (PDF/Word‑like) com enunciado organizado por pontos e espaço para os alunos colarem prints do resultado, ou ficas só com o texto do enunciado e solução para reutilizar no teu próprio template?
<span style="display:none">[^3_10][^3_11][^3_12][^3_13][^3_14][^3_15][^3_8][^3_9]</span>

<div align="center">⁂</div>

[^3_1]: https://uds.com.br/blog/linguagens-desenvolvimento-de-apps-android-e-ios/

[^3_2]: https://developer.android.com/get-started/overview?hl=pt-br

[^3_3]: https://github.com/braga-git/cursoemvideo-projeto-android

[^3_4]: https://www.devmedia.com.br/html5-video-tutorial/28790

[^3_5]: https://tecnoblog.net/responde/o-que-e-android-conheca-a-historia-do-sistema-operacional-movel-mais-popular-do-mundo/

[^3_6]: https://tek.sapo.pt/mobile/android/artigos/android-15-anos-de-evolucao-do-sistema-operativo-com-muitas-versoes-e-sobremesas-pelo-meio

[^3_7]: https://www.psafe.com/blog/android-evolucao-sistema-versoes/

[^3_8]: https://lucsasl.github.io/HTML5-CSS3-PTBR/

[^3_9]: https://guiadehtmlcssjs.com.br/material-de-apoio/17 - Primeiro mini-projeto.pdf

[^3_10]: https://www.youtube.com/watch?v=xS2D9x8odoE

[^3_11]: https://github.com/techmateus/html-css

[^3_12]: https://www.jotform.com/pt/blog/plataformas-de-desenvolvimento-de-baixo-codigo/

[^3_13]: https://www.youtube.com/watch?v=MnznvoNuy-I

[^3_14]: https://www.hostmidia.com.br/blog/o-que-e-android/

[^3_15]: https://www.dio.me/articles/30-sites-de-desafios-para-treinar-e-praticar-logica-de-programacao

