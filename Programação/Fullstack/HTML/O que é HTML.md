### O que é HTML?

HTML é uma linguagem de marcação que permite estruturar conteúdo na web. Ela é usada para criar elementos como textos, imagens, links e muito mais.

### Estrutura Básica de um Documento HTML

Um documento HTML tem uma estrutura básica. Aqui está um exemplo simples:

```html
<!DOCTYPE html>
<html lang="pt-BR"> 
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Título da Página</title>
</head>
<body>
	<h1>Bem-vindo ao HTML!</h1>
	<p>Este é um parágrafo de texto.</p>
	<a href="https://www.exemplo.com">Clique aqui para visitar um site</a> </body> </html>
```
```
```
### Explicação da Estrutura

1. **`<!DOCTYPE html>`**: Declara que este documento é um arquivo HTML5.
2. **`<html>`**: A [[Tag]] raiz que envolve todo o conteúdo da página.
3. **`<head>`**: Contém informações sobre o documento, como o título e os metadados.
    - **`<meta charset="UTF-8">`**: Define a codificação de caracteres.
    - **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Define a responsividade da página.
    - **`<title>`**: O título da página que aparece na aba do navegador.
4. **`<body>`**: Onde o conteúdo visível da página é colocado.
    - **`<h1>`**: Um cabeçalho principal.
    - **`<p>`**: Um parágrafo de texto.
    - **`<a>`**: Um link que pode ser clicado.

### Elementos HTML Comuns

- **Cabeçalhos**: `<h1>` a `<h6>` (h1 é o mais importante, h6 é o menos importante).
- **Parágrafos**: `<p>`.
- **Listas**:
    - Ordenadas: `<ol>` e `<li>`.
    - Não ordenadas: `<ul>` e `<li>`.
- **Imagens**: `<img src="url_da_imagem" alt="Texto alternativo">`.
- **Links**: `<a href="url">Texto do link</a>`.