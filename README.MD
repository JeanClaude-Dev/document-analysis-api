# 📄 Document Analysis API

API REST desenvolvida com **Node.js**, **Fastify** e **TypeScript** para simular um serviço de análise de documentos.

---

# Tecnologias utilizadas

* Node.js
* Fastify
* TypeScript
* tsx
* tsup

---

# Funcionalidades

A API permite:

* Listar documentos cadastrados
* Buscar documento por ID
* Simular o envio de um documento para análise
* Atualizar o status da análise
* Remover documentos

Todos os dados são armazenados em memória, não sendo utilizado banco de dados, mantendo a simplicidade.

---

# Estrutura do Projeto

```
src
 └── server.ts
```

---

# Endpoints

## GET /documents

Lista todos os documentos.

---

## GET /documents/:id

Retorna um documento pelo ID.

---

## POST /documents

Simula o envio de um documento.

Exemplo:

```json
{
    "fileName":"Curriculo.pdf",
    "category":"RH"
}
```

---

## PUT /documents/:id/status

Atualiza o status da análise.

Exemplo:

```json
{
    "status":"Analisado"
}
```

---

## DELETE /documents/:id

Remove um documento.

---

# Executando o projeto

Clone o repositório

```bash
git clone URL_DO_SEU_REPOSITORIO
```

Entre na pasta

```bash
cd document-analysis-api
```

Instale as dependências

```bash
npm install
```

Execute em modo desenvolvimento

```bash
npm run start:dev
```

Servidor disponível em:

```
http://localhost:3333
```

---

# Autor

Jean Claude Barreto
