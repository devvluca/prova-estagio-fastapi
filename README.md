# Gestor de Empresas e Obrigações Acessórias 🚀

API desenvolvida para gerenciar empresas e suas obrigações acessórias. Feita com **FastAPI**, **SQLAlchemy** e **PostgreSQL**, essa aplicação permite cadastrar empresas, consultar seus dados e gerenciar as obrigações que precisam ser cumpridas.

## 🚀 Endpoints Disponíveis

### Empresas
- **POST /empresas/**: Cadastra uma nova empresa.
- **GET /empresas/{empresa_id}**: Consulta uma empresa pelo ID.

### Obrigações Acessórias
- **POST /obrigacoes/**: Cadastra uma nova obrigação acessória.
- **GET /obrigacoes/{obrigacao_id}**: Consulta uma obrigação acessória pelo ID.


## 🧰 Tecnologias Utilizadas

- **FastAPI**: Framework para construção da API.
- **SQLAlchemy**: ORM para interação com o banco de dados.
- **PostgreSQL**: Banco de dados relacional.
- **Pydantic**: Validação de dados.
- **Uvicorn**: Servidor ASGI para rodar a aplicação.


## 📝 Exemplo de Uso

### Cadastrar uma Empresa 
```bash
curl -X 'POST' \
  'http://localhost:8000/empresas/' \
  -H 'Content-Type: application/json' \
  -d '{
  "nome": "Empresa Teste",
  "cnpj": "12.345.678/0001-99",
  "endereco": "Rua Teste, 123",
  "email": "contato@empresateste.com",
  "telefone": "11987654321"
}'
```

### Consultar uma Empresa
```bash
curl -X 'GET' \
  'http://localhost:8000/empresas/1'
