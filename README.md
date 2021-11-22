# EJS-Instação e Configuração da Partials
### Criação e inserção do conteúdo da pasta Partials

Vamos dar prosseguimento criando dentro da pasta views uma pasta chamada **partials.**

Dentro da partials, vamos criar 2 arquivos com a extensão .ejs.

***header.ejs***

```html
<!DOCTYPE html>
<head>
    <title>EJS</title>
</head>
<body>
    <p>Este é um arquivo header EJS</p>
</body>
</html>
```

***footer.ejs***

```html
<!DOCTYPE html>
<head>
    <title>EJS</title>
</head>
<body>
    <p>Este é um arquivo footer EJS</p>
</body>
</html>
```

Estes arquivos estarão presentes em todas as páginas da aplicação, evitando reescrita de código.
***

### Incluindo os arquivos da Partials na página principal

Para isso, vamos usar o código abaixo:

```html
<!DOCTYPE html>
<head>
    <title>EJS</title>
</head>
<body>
    <%- include('../views/partials/header.ejs')%>
    <h1>Este é um arquivo EJS</h1>
    <%- include('../views/partials/footer.ejs')%>
</body>
</html>
```

**Definições das Tags utilizadas no EJS**

**<%-** usado para inserir código js sem saída para o html.<br/>
**<%=** usado para exibir informação no html.<br/>
**%>**  usado para fechamento simples de tag.<br/>
