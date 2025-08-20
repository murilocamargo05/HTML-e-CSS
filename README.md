# 📘 Introdução ao HTML

## O que é HTML?
**HTML (HyperText Markup Language)** é a **linguagem de marcação** utilizada para estruturar páginas da web.  
Ele não é uma linguagem de programação, mas sim um conjunto de **tags** que organizam e descrevem o conteúdo da página (textos, imagens, links, formulários, etc.).

---

## 🔖 O que são Tags?
As **tags** são instruções utilizadas no HTML para marcar e organizar elementos dentro de uma página.  
Elas geralmente aparecem em pares:

```html
<p>Esse é um parágrafo</p>
```

- **Abertura:** `<p>`  
- **Fechamento:** `</p>`  
- **Conteúdo:** "Esse é um parágrafo"

### Principais Tags Básicas
- `<html>` → define o início do documento HTML.
- `<head>` → contém metadados (título, estilos, scripts).
- `<body>` → contém o conteúdo visível da página.
- `<h1>` até `<h6>` → títulos e subtítulos.
- `<p>` → parágrafos de texto.
- `<a>` → links.
- `<img>` → imagens.
- `<br>` → quebra de linha.
- `<hr>` → linha horizontal (separador).
- `<span>` → marca trechos de texto sem alterar a estrutura.
- `<div>` → container genérico para agrupar elementos.

---

## 🏷️ O que são Atributos?
Os **atributos** fornecem informações adicionais sobre as tags.  
Eles são sempre escritos **dentro da tag de abertura**.

Exemplo:
```html
<img src="imagem.jpg" alt="Descrição da imagem" width="200">
```

### Principais Atributos
- `class` → usado para aplicar estilos CSS ou selecionar elementos com JavaScript.
- `id` → identificador único para um elemento.
- `style` → permite aplicar estilos CSS diretamente.
- `lang` → define o idioma do conteúdo (`<html lang="pt-BR">`).
- `title` → mostra um texto quando o mouse passa sobre o elemento.
- `alt` → descrição alternativa em imagens (essencial para acessibilidade).
- `align` → define alinhamento (obsoleto, use CSS).
- `width` e `height` → definem largura e altura (usado em imagens, vídeos, etc.).

---

## 📐 Tags Estruturais
Essas tags são usadas para organizar a **estrutura semântica** da página:

- `<header>` → cabeçalho (logotipo, menus, título).
- `<main>` → conteúdo principal da página.
- `<article>` → conteúdo independente (artigos, posts, notícias).
- `<nav>` → seção de navegação (menus, links importantes).
- `<aside>` → conteúdo lateral (informações extras, anúncios).
- `<footer>` → rodapé (informações de contato, direitos autorais).
- `<div>` → container genérico.
- `<ul>` → lista não ordenada (com marcadores).
- `<ol>` → lista ordenada (numerada).
- `<li>` → item de lista.

---

## 📝 Tags de Títulos e Texto
- `<h1>` até `<h6>` → definem títulos, do mais importante (`h1`) ao menos importante (`h6`).
- `<p>` → parágrafo de texto.
- `<span>` → destaque de parte do texto sem alterar a linha.
- `<i>` → texto em itálico.
- `<br>` → quebra de linha.

Exemplo:
```html
<h1>Título Principal</h1>
<p>Esse é um <span>parágrafo</span> com <i>itálico</i>.</p>
```

---

## 🖊️ Criando Formulários
Os **formulários** permitem coletar informações dos usuários.  
Eles são criados com a tag `<form>`.

### Estrutura básica:
```html
<form action="/enviar-dados" method="post">
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome" placeholder="Digite seu nome">
  
  <label for="email">E-mail:</label>
  <input type="email" id="email" name="email" placeholder="Digite seu e-mail">
  
  <label for="mensagem">Mensagem:</label>
  <textarea id="mensagem" name="mensagem" rows="5"></textarea>
  
  <label for="curso">Curso:</label>
  <select id="curso" name="curso">
    <option value="html">HTML</option>
    <option value="css">CSS</option>
    <option value="js" disabled>JavaScript (em breve)</option>
  </select>
  
  <button type="submit">Enviar</button>
</form>
```

### Principais Elementos e Atributos de Formulário
- `<form action="" method="">` → define para onde os dados serão enviados.
- `<label>` → rótulo de um campo.
- `for` → associa o rótulo a um input (mesmo valor do `id`).
- `<input>` → campo de entrada.
  - `type` → define o tipo (`text`, `email`, `password`, `number`, `checkbox`, `radio`, etc.).
  - `name` → nome do campo (usado no backend).
  - `placeholder` → texto de dica dentro do campo.
  - `value` → valor inicial do campo.
  - `id` → identificador único.
- `<select>` e `<option>` → lista suspensa de opções.
- `disabled` → desabilita um campo.
- `<textarea rows="5">` → campo de texto longo (multilinha).
- `<button>` → botão (pode ser `submit`, `reset` ou `button`).
---
