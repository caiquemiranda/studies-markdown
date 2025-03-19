# 💡 Dicas e Boas Práticas para Markdown

Este guia compartilha dicas práticas e convenções recomendadas para escrever documentos Markdown mais limpos, consistentes e eficientes.

## Organização de Documentos

### Estrutura Hierárquica Clara

- Use cabeçalhos hierarquicamente (`#`, `##`, `###`) sem pular níveis
- Evite mais de um cabeçalho de nível 1 (`#`) por documento
- Mantenha uma estrutura lógica do documento

### Quebras de Seção

Considere usar linhas horizontais (`---`) para separar seções principais:

```markdown
## Seção 1

Conteúdo da seção 1...

---

## Seção 2

Conteúdo da seção 2...
```

## Formatação de Texto

### Consistência em Ênfases

Escolha uma convenção e mantenha-a consistente:
- Para itálico: `*itálico*` ou `_itálico_` (escolha um e use-o consistentemente)
- Para negrito: `**negrito**` ou `__negrito__` (escolha um e use-o consistentemente)

### Espaçamento

- Deixe uma linha em branco antes de cabeçalhos e depois de parágrafos
- Separe blocos de código e listas do resto do texto com linhas em branco
- Não use espaços excessivos ou linhas em branco desnecessárias

## Links e Referências

### URLs Longas

Para URLs longas, use links de referência para manter o texto principal limpo:

```markdown
Veja [este artigo][artigo-ref] para mais informações.

[artigo-ref]: https://exemplo.com/um-artigo-com-url-muito-longa-e-complicada-que-quebraria-a-legibilidade-do-texto
```

### Links para Arquivos Locais

Para links para outros arquivos no mesmo repositório, use caminhos relativos:

```markdown
Veja o [documento de instalação](./docs/instalacao.md) para instruções.
```

### Ancoragem em Documentos

Crie links para seções específicas do documento usando âncoras automáticas:

```markdown
[Volte ao topo](#dicas-e-boas-práticas-para-markdown)
```

O ID da âncora é criado a partir do texto do cabeçalho (em minúsculas, espaços convertidos em hifens, caracteres especiais removidos).

## Listas

### Indentação Consistente

- Use 2 ou 4 espaços para indentação (seja consistente)
- Mantenha itens semelhantes alinhados (especialmente em listas aninhadas)

### Numeração em Listas Ordenadas

No Markdown, você pode usar `1.` para todos os itens, e eles serão renderizados em ordem:

```markdown
1. Primeiro item
1. Segundo item
1. Terceiro item
```

Entretanto, para melhor manutenção, é recomendável numerar manualmente:

```markdown
1. Primeiro item
2. Segundo item
3. Terceiro item
```

## Imagens

### Texto Alternativo

Sempre inclua texto alternativo descritivo para acessibilidade:

```markdown
![Descrição detalhada da imagem](caminho/para/imagem.jpg)
```

### Dimensionamento (quando HTML é permitido)

```markdown
<img src="imagem.jpg" alt="Descrição" width="300" height="200">
```

## Tabelas

### Formatação Legível

Alinhe as barras verticais para melhorar a legibilidade no código-fonte:

```markdown
| Nome    | Idade | Cargo          |
|---------|-------|----------------|
| Maria   | 34    | Desenvolvedora |
| João    | 29    | Designer       |
| Carolina| 41    | Gerente        |
```

### Tabelas Simples

Mantenha as tabelas simples. Se precisar de estruturas complexas, considere outras soluções ou HTML.

## Código

### Especifique a Linguagem

Sempre especifique a linguagem do código para realce adequado:

```markdown
```python
def hello():
    print("Hello World")
```
```

### Código Inline

Use código inline (``) para nomes de funções, variáveis, comandos ou valores no texto:

```markdown
Use a função `print()` para exibir o valor da variável `nome`.
```

## Padronização

### Arquivo README.md

Todo projeto deve ter um arquivo README.md na raiz com pelo menos:

- Nome e descrição do projeto
- Instruções de instalação
- Como usar/executar
- Licença (se aplicável)

### Arquivos de Documentação

Para projetos maiores, estruture a documentação em múltiplos arquivos:

```
docs/
  ├─ instalacao.md
  ├─ uso.md
  ├─ api.md
  └─ solucao-problemas.md
```

## Práticas Específicas para GitHub

### Issue e PR Templates

Crie templates para issues e pull requests:

```markdown
## Descrição do Problema
[descrição clara e concisa]

## Comportamento Esperado
[o que deveria acontecer]

## Comportamento Atual
[o que está acontecendo]

## Passos para Reproduzir
1. [primeiro passo]
2. [segundo passo]
3. [e assim por diante...]
```

### GitHub Actions Workflows

Documente seus workflows do GitHub Actions com comentários claros.

## Boas Práticas para Escrita Técnica

### Seja Conciso

- Use frases curtas e diretas
- Evite jargões desnecessários
- Elimine palavras supérfluas

### Use Voz Ativa

- **Bom**: "O sistema processa os dados"
- **Evite**: "Os dados são processados pelo sistema"

### Seja Consistente com Terminologia

- Use os mesmos termos para os mesmos conceitos
- Evite sinônimos para termos técnicos

## Ferramentas para Melhorar seu Markdown

- **Linters**: [markdownlint](https://github.com/DavidAnson/markdownlint)
- **Formatadores**: [Prettier](https://prettier.io/)
- **Editores com Preview**: VS Code, Typora, Obsidian
- **Verificadores de Links**: [markdown-link-check](https://github.com/tcort/markdown-link-check)

## Próximos Passos

Para ver os conceitos aplicados em situações reais, confira nossos [exemplos práticos](exemplos-praticos.md).

---

[← Voltar ao Índice](README.md) 