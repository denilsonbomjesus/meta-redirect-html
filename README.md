# meta-redirect-html

Este repositório contém um exemplo para realizar **redirecionamentos automáticos de páginas** usando **meta tags** em HTML. Através do uso da tag `<meta http-equiv="refresh">`, é possível configurar redirecionamentos de uma página para outra, com ou sem atraso.

## 💡 O que é um redirecionamento meta?

O redirecionamento **meta** no HTML é uma técnica simples de redirecionamento de páginas utilizando a tag `<meta http-equiv="refresh">`. Essa tag permite que você defina um tempo de espera antes de redirecionar o visitante para uma nova URL.

Exemplo de um redirecionamento com 5 segundos de atraso:

```html
<head>
    <meta http-equiv="refresh" content="5;url=https://www.exemplo.com">
</head>
```

Neste caso, após 5 segundos, o navegador irá redirecionar o usuário para `https://www.exemplo.com`.

## 🚀 Funcionalidades

- Redirecionamento simples de uma página para outra.
- Suporte a redirecionamentos com atraso customizável.
- Exemplos prontos de uso de `<meta http-equiv="refresh">` em diversos cenários.

## ⚙️ Como usar

### Usando a tag `<meta http-equiv="refresh">`

Para adicionar um redirecionamento em sua página HTML, basta incluir a seguinte tag dentro da seção `<head>` do seu documento:

```html
<head>
    <meta http-equiv="refresh" content="TEMPO;url=URL_DE_DESTINO">
</head>
```

- **TEMPO**: O número de segundos que a página deve aguardar antes de redirecionar (pode ser 0 para redirecionamento imediato).
- **URL_DE_DESTINO**: A URL para onde o visitante será redirecionado.

Exemplo com 5 segundos de atraso:

```html
<head>
    <meta http-equiv="refresh" content="5;url=https://www.exemplo.com">
</head>
```

### Usando com JavaScript (caso precise de controle adicional)

Você também pode usar JavaScript para adicionar redirecionamentos de maneira programática:

```javascript
setTimeout(function(){
    window.location.href = "https://www.exemplo.com";
}, 5000); // 5000ms = 5 segundos
```
