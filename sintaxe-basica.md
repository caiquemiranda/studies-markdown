# 📝 Sintaxe Básica do Markdown

Este guia cobre os elementos básicos da sintaxe Markdown que você usará com mais frequência.

## Cabeçalhos

Os cabeçalhos são criados usando o símbolo `#` seguido de um espaço. O número de `#` determina o nível do cabeçalho:

```markdown
# Cabeçalho nível 1
## Cabeçalho nível 2
### Cabeçalho nível 3
#### Cabeçalho nível 4
##### Cabeçalho nível 5
###### Cabeçalho nível 6
```

Resultado:
# Cabeçalho nível 1
## Cabeçalho nível 2
### Cabeçalho nível 3
#### Cabeçalho nível 4
##### Cabeçalho nível 5
###### Cabeçalho nível 6

## Parágrafos e Quebras de Linha

Para criar parágrafos, simplesmente separe o texto com uma linha em branco:

```markdown
Este é o primeiro parágrafo.

Este é o segundo parágrafo.
```

Para criar uma quebra de linha (sem criar um novo parágrafo), termine a linha com dois ou mais espaços e depois pressione Enter:

```markdown
Esta linha termina com dois espaços  
Esta é a próxima linha.
```

## Ênfase (Itálico e Negrito)

### Itálico

```markdown
*Este texto está em itálico*
_Este texto também está em itálico_
```

Resultado: *Este texto está em itálico* e _Este texto também está em itálico_

### Negrito

```markdown
**Este texto está em negrito**
__Este texto também está em negrito__
```

Resultado: **Este texto está em negrito** e __Este texto também está em negrito__

### Combinado

```markdown
**Este texto está em negrito e _parte dele em itálico_**
```

Resultado: **Este texto está em negrito e _parte dele em itálico_**

## Listas

### Listas Não Ordenadas

Use asteriscos, sinais de adição ou hifens como marcadores:

```markdown
* Item 1
* Item 2
  * Subitem 2.1
  * Subitem 2.2
* Item 3

- Item 1
- Item 2
- Item 3

+ Item 1
+ Item 2
+ Item 3
```

Resultado:
* Item 1
* Item 2
  * Subitem 2.1
  * Subitem 2.2
* Item 3

### Listas Ordenadas

Use números seguidos de ponto:

```markdown
1. Primeiro item
2. Segundo item
   1. Subitem 2.1
   2. Subitem 2.2
3. Terceiro item
```

Resultado:
1. Primeiro item
2. Segundo item
   1. Subitem 2.1
   2. Subitem 2.2
3. Terceiro item

## Links

### Link Básico

```markdown
[Texto do link](https://www.exemplo.com)
```

Resultado: [Texto do link](https://www.exemplo.com)

### Link com Título

```markdown
[Texto do link](https://www.exemplo.com "Título do link")
```

Resultado: [Texto do link](https://www.exemplo.com "Título do link")

### URL e Email Diretos

```markdown
<https://www.exemplo.com>
<email@exemplo.com>
```

Resultado: <https://www.exemplo.com> e <email@exemplo.com>

## Imagens

```markdown
![Texto alternativo](caminho/para/imagem.jpg)
![Texto alternativo](caminho/para/imagem.jpg "Título da imagem")
```

## Citações (Blockquotes)

```markdown
> Esta é uma citação.
>
> Esta é a segunda linha da citação.
```

Resultado:
> Esta é uma citação.
>
> Esta é a segunda linha da citação.

### Citações Aninhadas

```markdown
> Esta é a citação externa
>
> > Esta é a citação aninhada
```

Resultado:
> Esta é a citação externa
>
> > Esta é a citação aninhada

## Código

### Código Inline

```markdown
Use a função `print()` para exibir texto.
```

Resultado: Use a função `print()` para exibir texto.

### Blocos de Código

```markdown
    // Indentados com 4 espaços
    function exemplo() {
        return "olá, mundo";
    }
```

Ou usando cercas de código (```) para destacar blocos:

````markdown
```javascript
function exemplo() {
    return "olá, mundo";
}
```
````

## Linhas Horizontais

Crie linhas horizontais com três ou mais asteriscos, hifens ou sublinhados:

```markdown
***
---
___
```

Resultado:

---

## Caracteres de Escape

Use a barra invertida (`\`) para escapar caracteres que têm significado especial em Markdown:

```markdown
\* Este não é um item de lista
\# Isto não é um cabeçalho
```

## Próximos Passos

Agora que você domina a sintaxe básica do Markdown, explore a [sintaxe avançada](sintaxe-avancada.md) para recursos como tabelas, notas de rodapé e muito mais.

---

[← Voltar ao Índice](README.md) 