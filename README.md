# Desenvolvimento-de-Sistemas

```markdown
# APIs REST – C# (.NET) e Python

## Descrição

Este repositório apresenta duas implementações de **API REST** desenvolvidas em linguagens diferentes: **C# com .NET** e **Python com Flask**. O objetivo do projeto é demonstrar, de forma prática, o funcionamento da **arquitetura cliente-servidor** e a utilização do **protocolo HTTP** para comunicação entre aplicações.

Cada API disponibiliza **dados fictícios através de endpoints HTTP**, retornando as informações no formato **JSON**. Dessa forma, diferentes aplicações clientes podem consumir esses dados por meio de requisições HTTP.

O projeto foi desenvolvido para demonstrar como o mesmo conceito de **API REST** pode ser implementado utilizando diferentes tecnologias e linguagens de programação.

---

# Estrutura do Repositório

```
````
projeto-api
│
├── api-csharp
│   ├── Controllers
│   │     └── ProdutosController.cs
│   ├── Models
│   │     └── Produto.cs
│   ├── Program.cs
│   └── ApiProdutos.csproj
│
└── api-python
└── api.py
```
````

### Descrição das Pastas

| Pasta | Descrição |
|------|-----------|
| **api-csharp** | Implementação da API REST utilizando **C# e ASP.NET Core** |
| **api-python** | Implementação da API REST utilizando **Python e Flask** |

---

# API em C# (.NET)

A API em C# foi desenvolvida utilizando **ASP.NET Core Web API**. Ela disponibiliza endpoints que retornam dados fictícios de produtos em formato **JSON**.

### Tecnologias utilizadas

- C#
- .NET
- ASP.NET Core Web API
- Swagger / OpenAPI

### Executando a API

Acesse a pasta da API:

```bash
cd api-csharp
````

Execute o projeto:

```bash
dotnet run
```

Após iniciar, a API estará disponível em:

```
http://localhost:5143
```

Swagger:

```
http://localhost:5143/swagger
```

---

# API em Python

A segunda implementação da API foi desenvolvida utilizando **Python** com o framework **Flask**, que permite criar APIs REST de forma simples e rápida.

### Tecnologias utilizadas

* Python
* Flask

### Executando a API

Acesse a pasta da API:

```bash
cd api-python
```

Instale as dependências:

```bash
pip install flask
```

Execute a API:

```bash
python api.py
```

A API ficará disponível em:

```
http://localhost:5000
```

---

# Exemplo de Endpoint

Ambas as APIs possuem um endpoint semelhante para listar produtos.

### Requisição

```
GET /api/produtos
```

### Exemplo de resposta

```json
[
  {
    "id": 1,
    "nome": "Notebook",
    "preco": 3500
  },
  {
    "id": 2,
    "nome": "Mouse",
    "preco": 80
  },
  {
    "id": 3,
    "nome": "Teclado",
    "preco": 150
  }
]
```

---

# Arquitetura Cliente-Servidor

O funcionamento das APIs segue o modelo **cliente-servidor**, no qual:

| Etapa | Descrição                                           |
| ----- | --------------------------------------------------- |
| 1     | O cliente envia uma requisição HTTP para o servidor |
| 2     | O servidor processa a requisição                    |
| 3     | A API retorna os dados em formato JSON              |
| 4     | O cliente recebe e utiliza as informações           |

---

# Objetivo do Projeto

Este projeto foi desenvolvido com o objetivo de:

* Compreender a **arquitetura cliente-servidor**
* Demonstrar o uso do **protocolo HTTP**
* Implementar **APIs REST em diferentes linguagens**
* Comparar implementações utilizando **C# e Python**

---

# Autor
````
Nome: Victor Santos Barcelos
Curso: Ciências da Computação
Disciplina: Desenvolvimento de Sistemas 
Professor: Daniel Linhares Lim Apo
````
