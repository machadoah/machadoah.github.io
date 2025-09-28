---
date: 2025-09-27
tags: fastapi
author: antonio
series: FastAPI
title: FastAPI - Setup Inicial
description: Setup inicial de um projeto com FastAPI!
banner_image: media/fastapi/fastapi-blog.png
extra:
  mermaid: true
  math: true
---

## 👋🏼 Olá, mundo

Olá galera! Como estão? Hoje vamos fazer o setup inicial de um projeto com FastAPI! 🚀

Antes de tudo, espero que tenham visto o post anterior onde eu faço uma introdução ao FastAPI, caso não tenha visto, [clique aqui](https://machadoah.github.io/series-fastapi.html) para ler! 😉

Hoje o objetivo é fazer um setup simples, mas que já nos permita criar uma API básica e ir evoluindo ela nos próximos posts! Vamos lá?

### Instalação e Setup Inicial

Assim, quero fazer um pequeno disclaimer: Eu recomendo fortemente que você utilize um ambiente [UNIX](https://pt.wikipedia.org/wiki/Unix), que pode ser o Linux ou o MacOS. Caso você utilize Windows, recomendo que utilize o [WSL](https://learn.microsoft.com/pt-br/windows/wsl/install) para ter uma experiência mais próxima do UNIX.

Então, vamos lá!

#### Instalação do Python

Primeiro, precisamos ter o Python instalado. Você pode verificar se já tem o Python instalado e qual a versão com o comando:

```bash
python3 --version
```

Se você não tiver o Python instalado, você pode baixar e instalar a versão mais recente do Python 3 a partir do site oficial: [https://www.python.org/downloads/](https://www.python.org/downloads/).

Mas, eu não recomendo instalar o Python diretamente no seu sistema operacional. Eu recomendo que você utilize o [UV](https://docs.astral.sh/uv/#installation) para gerenciar suas versões do Python. Você pode instalar o UV com o comando:

```bash
curl -sSL https://install.astral.sh | sh
```

E depois, você consegue instalar a versão mais recente do Python com o comando:

```bash
uv python install 3.13
```

Recomendo conhecer melhor o UV, e a instalação do Python com ele, na [documentação oficial](https://docs.astral.sh/uv/guides/install-python/).

#### Instalando o FastAPI

Antes de instalar o FastAPI, recomendo que você crie um ambiente virtual para o seu projeto. Isso ajuda a manter as dependências do projeto isoladas e evita conflitos com outras bibliotecas que você possa ter instalado globalmente.

Você pode criar um ambiente virtual com o comando a seguir, no diretório do seu projeto:

```bash
uv v
```

Sendo assim, ative o ambiente virtual com o comando:

```bash
source .venv/bin/activate
```

Agora, você pode instalar o FastAPI com o comando:

```bash
uv add fastapi --extra standard
```

E com isso você já tem o FastAPI instalado! 🎉

Caso, esteja utilizando o `UV`, poderá ver as dependências instaladas no arquivo `pyproject.toml`.

```toml
[project]
name = "backend"
version = "0.1.0"
description = "Add your description here"
readme = "README.md"
requires-python = ">=3.13"
dependencies = [
    "fastapi[standard]>=0.116.1", # 👈🏼 Essa linha aqui foi adicionada
]
```

### API Endpoint

No FastAPI, criar um endpoint é simples e direto. Vamos criar um arquivo chamado `main.py` e adicionar o seguinte código:

```python
def get_book():
    return {
        "name": "Esaú e Jacó",
        "author": "Machado de Assis"
    }
```

Maaas, isso não é um endpoint ainda! Para transformar essa função em um endpoint, precisamos usar o FastAPI. Vamos importar o FastAPI e criar uma instância da aplicação:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/book")
def get_book():
    return {
        "name": "Esaú e Jacó",
        "author": "Machado de Assis"
    }
```

Agora que definimos o endpoint, podemos rodar a aplicação com o comando:

```bash
uv run fastapi dev main.py
```

Agora, podemos acessar o endpoint no navegador ou usar uma ferramenta como o [Postman](https://www.postman.com/) ou [Insomnia](https://insomnia.rest/) para fazer uma requisição GET para `http://localhost:8000/book`.

Mas aqui, vou usar o `httpie`, que é uma ferramenta de linha de comando para fazer requisições HTTP. Você pode instalar o `httpie` com o comando:

```bash
http GET http://127.0.0.1:8000/book
```

E com isso, você verá a resposta JSON com os detalhes do livro:

```json
{
    "name": "Esaú e Jacó",
    "author": "Machado de Assis"
}
```

### Próximos Passos

E é isso! Agora você tem um setup inicial de um projeto com FastAPI e um endpoint básico funcionando! 🎉

Nos próximos posts, vamos explorar mais funcionalidades do FastAPI, como parâmetros de rota, validação de dados, autenticação, entre outros tópicos interessantes! Fique ligado! 😉
