# 🔍 Sintaxe Avançada do Markdown

Este guia explora recursos avançados do Markdown, disponíveis em várias implementações e extensões populares como GitHub Flavored Markdown (GFM), MultiMarkdown e Markdown Extra.

## Tabelas

As tabelas são suportadas em muitas variantes do Markdown:

```markdown
| Cabeçalho 1 | Cabeçalho 2 | Cabeçalho 3 |
|-------------|-------------|-------------|
| Célula 1    | Célula 2    | Célula 3    |
| Linha 2     | Exemplo     | Texto       |
```

Resultado:

| Cabeçalho 1 | Cabeçalho 2 | Cabeçalho 3 |
|-------------|-------------|-------------|
| Célula 1    | Célula 2    | Célula 3    |
| Linha 2     | Exemplo     | Texto       |

### Alinhamento em Tabelas

Você pode alinhar o texto nas colunas usando dois pontos (`:`):

```markdown
| Alinhado à Esquerda | Centralizado | Alinhado à Direita |
|:--------------------|:------------:|-------------------:|
| Esquerda            | Centro       | Direita            |
| texto               | texto        | texto              |
```

Resultado:

| Alinhado à Esquerda | Centralizado | Alinhado à Direita |
|:--------------------|:------------:|-------------------:|
| Esquerda            | Centro       | Direita            |
| texto               | texto        | texto              |

## Listas de Tarefas

Comum no GitHub Flavored Markdown:

```markdown
- [x] Tarefa concluída
- [ ] Tarefa pendente
- [ ] ~~Tarefa cancelada~~
```

Resultado:
- [x] Tarefa concluída
- [ ] Tarefa pendente
- [ ] ~~Tarefa cancelada~~

## Texto Riscado

```markdown
~~Este texto está riscado~~
```

Resultado: ~~Este texto está riscado~~

## Definição de Identificadores para Cabeçalhos

```markdown
## Meu Cabeçalho {#identificador-personalizado}
```

Isso permite criar links para seções específicas:

```markdown
[Link para o cabeçalho](#identificador-personalizado)
```

## Notas de Rodapé

Disponível em algumas variantes:

```markdown
Aqui está um texto com uma nota de rodapé[^1].

[^1]: Esta é a nota de rodapé.
```

Resultado:
Aqui está um texto com uma nota de rodapé[^1].

[^1]: Esta é a nota de rodapé.

## Abreviações

```markdown
*[HTML]: Hypertext Markup Language
*[W3C]: World Wide Web Consortium

O HTML é padronizado pelo W3C.
```

Quando hover sobre HTML ou W3C, a expansão aparecerá.

## Definição de Listas

```markdown
Termo
: Definição do termo
: Outra definição

Outro termo
: Definição do outro termo
```

Resultado:

Termo
: Definição do termo
: Outra definição

Outro termo
: Definição do outro termo

## Extensões de Realce de Sintaxe

O realce de sintaxe é especificado após as três crases iniciais de um bloco de código:

````markdown
```python
def hello_world():
    print("Hello, World!")
```

```json
{
  "nome": "João",
  "idade": 30
}
```
````

## Diagramas (Mermaid)

Algumas plataformas como GitHub suportam a sintaxe Mermaid para criar diagramas:

````markdown
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

## Matemática (LaTeX)

Muitas implementações suportam fórmulas matemáticas usando sintaxe LaTeX:

```markdown
Inline: $E=mc^2$

Bloco:
$$
\frac{d}{dx}e^x = e^x
$$
```

## Emojis

No GitHub e outras plataformas:

```markdown
:smile: :heart: :rocket:
```

Resultado: 😄 ❤️ 🚀

## Menções de Usuários (em plataformas sociais)

```markdown
@nome_do_usuario
```

## Destaque de Linha em Blocos de Código

```markdown
```python hl_lines="1 3"
print("Esta linha será destacada")
print("Esta linha não")
print("Esta linha será destacada novamente")
```
```

## Avisos/Alertas (GitHub)

```markdown
> [!NOTE]
> Esta é uma nota informativa.

> [!WARNING]
> Este é um aviso importante.

> [!TIP]
> Esta é uma dica útil.
```

## Inclusão de HTML

A maioria das implementações de Markdown permite usar HTML diretamente:

```markdown
<div style="background-color: yellow; padding: 10px;">
  Este é um <strong>conteúdo personalizado</strong> com HTML.
</div>
```

## Comentários

Você pode adicionar comentários que não serão renderizados:

```markdown
<!-- Este é um comentário que não aparecerá na visualização final -->
```

## Próximos Passos

Agora que você conhece recursos avançados do Markdown, é recomendável explorar as [dicas e boas práticas](dicas-boas-praticas.md) para melhorar ainda mais seus documentos.

---

[← Voltar ao Índice](README.md) 