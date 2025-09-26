---
date: 2025-08-31
tags: fastapi
author: antonio
series: FastAPI
# stream: draft
title: 01 - Introdução ao FastAPI e API
description: Compreenda o que é o FastAPI!
# slug: parametros # nome do arquivo sem a data
banner_image: media/fastapi-blog.png
extra:
  mermaid: true
  math: true
---

## 👋🏼 Olá, FastAPI

> [!WARNING] ⚡️
> Esse é o meu primeiro "post", relacionado ao [FastAPI](https://fastapi.tiangolo.com/)!

O FastAPI é um framework web moderno e de alto desempenho para construir APIs com Python. Ele é rápido, fácil de usar e oferece uma série de recursos que facilitam o desenvolvimento de APIs robustas e escaláveis.

Meu objetivo com esta série de posts é compartilhar conhecimentos e experiências sobre o desenvolvimento de APIs utilizando o FastAPI, abordando desde conceitos básicos até tópicos mais avançados. Espero que você aproveite e aprenda bastante com o conteúdo!

<!--
Fique à vontade para sugerir temas ou fazer perguntas nos comentários. Vamos juntos explorar o mundo do FastAPI e construir APIs incríveis!
-->

Quero passar por tópicos como:

- Introdução ao FastAPI e API
- Métodos HTTP no FastAPI
- Pydantic
- SQLModel
- AsyncIO
- PostgreSQL
- Autenticação e Autorização
- Alembic - Migrations
- Testes
- Docker
- ...

Entre outros!

Meu objetivo é trabalharmos como exemplos práticos e reais, com eventos, usuários, autenticação, banco de dados, deploy, etc.

O principal objetivo é termos conhecimento prático para desenvolver APIs RESTful utilizando o FastAPI, com boas práticas de desenvolvimento, segurança e performance.

### O que são REST APIs?

### O que é o FastAPI?

### Por que usar o FastAPI?

```python
# Importa a classe FastAPI do módulo fastapi
from fastapi import FastAPI

# Cria uma instância da aplicação FastAPI
app = FastAPI()

#        👇🏽 Aqui temos a rota que será acessada
@app.get("/")
async def read_root():
    return {"Hello": "World"}
```
