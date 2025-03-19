# 🛠️ Exemplos Práticos de Markdown

Este guia contém exemplos de aplicações reais do Markdown em diferentes contextos e plataformas.

## README para Projetos de Software

Um bom README é essencial para qualquer projeto open-source:

```markdown
# Nome do Projeto

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Build Status](https://travis-ci.org/usuario/projeto.svg?branch=master)](https://travis-ci.org/usuario/projeto)
[![Coverage](https://codecov.io/gh/usuario/projeto/branch/master/graph/badge.svg)](https://codecov.io/gh/usuario/projeto)

> Uma descrição concisa e clara do que o projeto faz.

## 📋 Pré-requisitos

- Node.js v14+
- MongoDB v4.4+
- NPM ou Yarn

## 🚀 Instalação

```bash
# Clone o repositório
git clone https://github.com/usuario/projeto.git

# Entre no diretório
cd projeto

# Instale as dependências
npm install
```

## ⚙️ Configuração

Crie um arquivo `.env` na raiz do projeto:

```
DATABASE_URL=mongodb://localhost:27017/meu_banco
API_KEY=sua_chave_api
```

## 🔍 Uso

```javascript
const projeto = require('projeto');

// Inicialize o projeto
const app = projeto.init();

// Execute a função principal
app.run();
```

## 🧪 Testes

```bash
npm test
```

## 🤝 Contribuição

1. Faça um Fork do projeto
2. Crie uma Branch para sua Feature (`git checkout -b feature/AmazingFeature`)
3. Adicione suas mudanças (`git add .`)
4. Comite suas mudanças (`git commit -m 'Add some AmazingFeature'`)
5. Faça Push da Branch (`git push origin feature/AmazingFeature`)
6. Abra um Pull Request

## 📝 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

## 📬 Contato

Seu Nome - [@seu_twitter](https://twitter.com/seu_twitter) - email@exemplo.com
```

## Documentação de API

Markdown é excelente para documentar APIs:

```markdown
# API de Usuários

Base URL: `https://api.exemplo.com/v1`

## Autenticação

Todas as requisições autenticadas devem incluir o cabeçalho:

```
Authorization: Bearer SEU_TOKEN_JWT
```

## Endpoints

### Listar Usuários

```
GET /users
```

**Parâmetros de consulta:**

| Parâmetro | Tipo    | Descrição                     |
|-----------|---------|-------------------------------|
| limit     | integer | Número máximo de resultados   |
| offset    | integer | Número de resultados a pular  |
| sort      | string  | Campo para ordenação          |

**Resposta:**

```json
{
  "total": 100,
  "users": [
    {
      "id": 1,
      "name": "João Silva",
      "email": "joao@exemplo.com",
      "created_at": "2023-01-01T00:00:00Z"
    },
    // ...
  ]
}
```

### Obter Usuário

```
GET /users/{id}
```

**Parâmetros de caminho:**

| Parâmetro | Tipo    | Descrição           |
|-----------|---------|---------------------|
| id        | integer | ID único do usuário |

**Resposta:**

```json
{
  "id": 1,
  "name": "João Silva",
  "email": "joao@exemplo.com",
  "created_at": "2023-01-01T00:00:00Z",
  "profile": {
    "bio": "Desenvolvedor Full Stack",
    "location": "São Paulo, Brasil"
  }
}
```

### Criar Usuário

```
POST /users
```

**Corpo da requisição:**

```json
{
  "name": "Maria Oliveira",
  "email": "maria@exemplo.com",
  "password": "senha_segura"
}
```

**Resposta:**

```json
{
  "id": 2,
  "name": "Maria Oliveira",
  "email": "maria@exemplo.com",
  "created_at": "2023-08-05T10:30:00Z"
}
```

## Códigos de Status

| Código | Descrição                                           |
|--------|-----------------------------------------------------|
| 200    | Sucesso                                             |
| 201    | Recurso criado com sucesso                          |
| 400    | Parâmetros inválidos ou ausentes                    |
| 401    | Não autenticado                                     |
| 403    | Permissão negada                                    |
| 404    | Recurso não encontrado                              |
| 500    | Erro interno do servidor                            |
```

## Documentação de Bibliotecas e Frameworks

```markdown
# Componente Button

Um botão reutilizável com vários estilos e tamanhos.

## Importação

```jsx
import { Button } from 'componentes-ui';
```

## Uso Básico

```jsx
<Button>Clique Aqui</Button>
<Button variant="primary" size="large">Enviar</Button>
<Button variant="danger" disabled>Excluir</Button>
```

## Props

| Prop       | Tipo                              | Padrão    | Descrição                      |
|------------|---------------------------------|-----------|--------------------------------|
| variant    | 'default' \| 'primary' \| 'danger' | 'default' | Estilo visual do botão         |
| size       | 'small' \| 'medium' \| 'large'     | 'medium'  | Tamanho do botão               |
| disabled   | boolean                           | false     | Define se o botão está desabilitado |
| onClick    | function                          | -         | Função chamada ao clicar       |
| children   | ReactNode                         | -         | Conteúdo do botão              |

## Exemplos

### Botão com ícone

```jsx
<Button>
  <Icon name="save" /> Salvar
</Button>
```

### Botão de carregamento

```jsx
<Button loading>Processando...</Button>
```
```

## Wiki de Projeto

Exemplo de uma página wiki para um projeto colaborativo:

```markdown
# 📚 Guia de Contribuição

Bem-vindo ao projeto! Este guia ajudará você a começar a contribuir.

## 🚀 Primeiros Passos

1. **Ambiente de Desenvolvimento**
   
   Confirme que você tem instalado:
   - Python 3.8+
   - Docker
   - VS Code (recomendado)

2. **Configuração Local**

   ```bash
   git clone https://github.com/org/projeto.git
   cd projeto
   python -m venv venv
   source venv/bin/activate  # ou venv\Scripts\activate no Windows
   pip install -r requirements.txt
   ```

3. **Executando Localmente**

   ```bash
   docker-compose up -d  # inicia dependências
   python manage.py migrate
   python manage.py runserver
   ```

## 🧪 Testes

Executamos três tipos de testes:

1. **Testes Unitários**
   ```bash
   pytest tests/unit/
   ```

2. **Testes de Integração**
   ```bash
   pytest tests/integration/
   ```

3. **Testes End-to-End**
   ```bash
   pytest tests/e2e/
   ```

## 📝 Diretrizes de Código

### Estilo de Código

Seguimos a [PEP 8](https://www.python.org/dev/peps/pep-0008/) para Python.

### Commits

Usamos commits semânticos:

- `feat:` - Nova funcionalidade
- `fix:` - Correção de bug
- `docs:` - Documentação
- `style:` - Formatação (não afeta o código)
- `refactor:` - Refatoração de código
- `test:` - Testes
- `chore:` - Tarefas de manutenção

### Pull Requests

- Use nosso template de PR
- Vincule issues relacionadas
- Adicione screenshots para mudanças visuais
- Certifique-se que os testes passam

## 🗂️ Estrutura do Projeto

```
projeto/
├── api/            # Endpoints da API
├── core/           # Lógica de negócio principal
├── config/         # Configurações
├── tests/          # Testes
│   ├── unit/
│   ├── integration/
│   └── e2e/
├── docs/           # Documentação adicional
└── scripts/        # Scripts utilitários
```
```

## Anotações e Notas de Estudo

```markdown
# 📖 Notas: Algoritmos de Ordenação

## Bubble Sort

- **Complexidade de tempo**: O(n²)
- **Espaço**: O(1)

### Algoritmo

1. Compare elementos adjacentes
2. Troque se estiverem na ordem errada
3. Repita até o final da lista
4. Repita os passos até que não sejam necessárias mais trocas

### Código

```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    return arr
```

### Prós e Contras

➕ Simples de implementar
➕ Funciona bem para listas quase ordenadas

➖ Ineficiente para grandes conjuntos de dados
➖ Desempenho pior que outros algoritmos

## Quick Sort

- **Complexidade média**: O(n log n)
- **Pior caso**: O(n²)
- **Espaço**: O(log n)

### Algoritmo

1. Escolha um elemento como pivô
2. Particione: elementos menores à esquerda, maiores à direita
3. Aplique recursivamente nos subconjuntos

### Código

```python
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quick_sort(left) + middle + quick_sort(right)
```

### Quando usar

- Conjuntos grandes de dados
- Quando o espaço extra não é um problema
- Quando o caso médio é mais importante que o pior caso
```

## Apresentação Técnica

```markdown
# Microsserviços vs. Monolitos

## Arquitetura Monolítica

![Diagrama de Monolito](./imagens/monolito.png)

### Características

- Uma única base de código
- Implantação como uma unidade
- Escala como um todo
- Geralmente compartilha banco de dados

### Vantagens

- Simplicidade de desenvolvimento
- Fácil debugging
- Menor complexidade operacional
- Melhor desempenho de comunicação interna

## Arquitetura de Microsserviços

![Diagrama de Microsserviços](./imagens/microsservicos.png)

### Características

- Serviços independentes
- Cada um com responsabilidade única
- Comunicação via APIs/mensagens
- Bancos de dados separados

### Vantagens

- Implantação independente
- Escalabilidade granular
- Isolamento de falhas
- Diversidade tecnológica

## Comparação

| Aspecto             | Monolito                | Microsserviços           |
|---------------------|-------------------------|--------------------------|
| Complexidade        | Baixa inicialmente      | Alta desde o início      |
| Velocidade inicial  | Rápido para começar     | Lento para iniciar       |
| Escala organizacional | Funciona para equipes pequenas | Melhor para equipes grandes |
| Resiliência         | Ponto único de falha    | Isolamento de falhas     |
| DevOps              | Requisitos simples      | Requisitos complexos     |

## Decisão

### Quando escolher Monolito

- Startups e MVPs
- Domínio não bem definido
- Equipes pequenas
- Requisitos simples de escala

### Quando escolher Microsserviços

- Aplicações complexas
- Equipes grandes ou múltiplas
- Alta necessidade de escala
- Requisitos de resiliência
```

## Resumo de Livro/Artigo

```markdown
# 📚 Resumo: "Clean Code" de Robert C. Martin

## 📌 Principais Conceitos

### Nomes Significativos

- Nomes devem revelar intenção
- Evite nomes genéricos (data, manager, processor)
- Evite abreviações
- Use substantivos para classes, verbos para métodos

**Exemplo:**
```java
// Ruim
public List<int[]> getThem() {
    List<int[]> list1 = new ArrayList<int[]>();
    for (int[] x : theList)
        if (x[0] == 4) list1.add(x);
    return list1;
}

// Bom
public List<Cell> getFlaggedCells() {
    List<Cell> flaggedCells = new ArrayList<Cell>();
    for (Cell cell : gameBoard)
        if (cell.isFlagged()) flaggedCells.add(cell);
    return flaggedCells;
}
```

### Funções Pequenas

- Funções devem fazer uma única coisa
- Devem ser pequenas (idealmente ≤ 20 linhas)
- Níveis de indentação: no máximo 1-2
- Poucos argumentos (idealmente ≤ 2)

### Comentários

- Bom código geralmente não precisa de comentários
- Comentários não devem compensar código ruim
- Use para explicar intenção, clarificar, alertar sobre consequências

### Formatação

- Consistência é fundamental
- Arquivos semelhantes, estrutura semelhante
- Declare variáveis próximas de seu uso
- Funções relacionadas devem estar próximas

## 💡 Técnicas Práticas

### Lei de Demeter

Uma função só deve chamar métodos de:
- O próprio objeto
- Objetos criados pela função
- Objetos passados como argumentos
- Objetos armazenados em variáveis de instância

### Tratamento de Erros

- Use exceções em vez de códigos de retorno
- Crie classes de exceção informativas
- Não retorne null
- Não passe null

### Testes Limpos

- Um conceito por teste
- F.I.R.S.T: Fast, Independent, Repeatable, Self-validating, Timely
- Padrão AAA: Arrange, Act, Assert

## 🔑 Citações Importantes

> "A única maneira de ir rápido é ir bem."

> "Deixe o código mais limpo do que você o encontrou."

> "Funções devem fazer uma coisa. Devem fazê-la bem. Devem fazer apenas ela."

## 🛠️ Aplicação Prática

O autor sugere o seguinte processo iterativo:

1. Faça funcionar
2. Faça funcionar corretamente
3. Faça funcionar bem (refatore)
4. Faça funcionar rápido (otimize se necessário)

## 📝 Conclusão

"Clean Code" não é apenas sobre técnicas específicas, mas sobre uma filosofia de desenvolvimento que valoriza a legibilidade, simplicidade e manutenção. O código limpo é aquele que pode ser facilmente entendido e modificado por qualquer desenvolvedor, não apenas por seu autor original.
```

---

[← Voltar ao Índice](README.md) 