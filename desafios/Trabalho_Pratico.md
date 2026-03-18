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


9. Área para vídeo sobre plataformas de desenvolvimento Android
```
- Dentro do `<main>`, criar uma secção (pode ser um `<section>` ou `<div>`) com o título “Plataformas de desenvolvimento para Android”.
```

- Inserir um vídeo:
    - Pode ser um `<iframe>` incorporando um vídeo do YouTube sobre plataformas/IDE para Android (ex.: Android Studio, Flutter, etc.).
    - Ou um `<video>` com ficheiro local (opcional).
- O vídeo deve estar centrado e ser responsivo: largura máxima 560px, ocupando 100% da largura disponível em ecrãs pequenos.

10. Área para lista da evolução histórica do Android

- Ainda dentro do `<main>`, criar outra secção com o título “Evolução histórica do Android”.
- Adicionar uma lista ordenada `<ol>` com pelo menos 5 itens, cada um com:
    - Ano ou versão (ex.: “2008 – Android 1.0”).
    - Pequena descrição (1 frase) da importância dessa versão (primeiro lançamento, mudança de interface, etc.).

***
Entrega:

- Ficheiro `desafio-simples.html`.
- Ficheiro `style.css`.
- Imagem usada (por exemplo na pasta `imagens/`).

***
