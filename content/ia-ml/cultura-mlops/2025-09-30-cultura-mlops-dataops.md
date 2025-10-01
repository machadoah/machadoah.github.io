---
date: 2025-09-30
tags: inteligencia-artificial, mlops, dataops, cultura
author: antonio
series: cultura-e-praticas-em-dataops-e-mlops
stream: draft
title: DataOps e MLOps - Fundamentos da Cultura em MLOps e DataOps
description: Introdução aos Fundamentos da Cultura em MLOps e DataOps
banner_image: media/mlops-blog.png
extra:
  mermaid: true
  math: true
---

## 👋🏽 Olá, Mundo

Bem-vindo a mais um artigo da série sobre Cultura e Práticas em DataOps e MLOps! 🚀

Agora que a gente já falou sobre DevOps, vamos entender o que é DataOps e MLOps, mas já adiantando, meio que essa é a evolução do DevOps, focado em dados e aprendizado de máquina.

Nesse artigo, vamos tentar manter as coisas simples e diretas, evitando jargões técnicos complicados. A ideia é que qualquer pessoa, mesmo sem muito conhecimento prévio, consiga entender os conceitos básicos de DataOps e MLOps.

Por conta disso, se você já é um expert no assunto, pode ser que ache o conteúdo um pouco básico demais. Mas tudo bem, a ideia aqui é ajudar quem está começando ou quer entender melhor esses conceitos.

Agora, bora lá!

> [!NOTE] 🧑🏽‍💻
> Outro ponto! Vamos tentar fazer analogias simples para facilitar o entendimento, então se algo parecer meio estranho ou engraçado, é por isso! 😄

### DataOps e MLOps

DataOps e MLOps são abordagens que aplicam os princípios e práticas do DevOps ao gerenciamento de dados e ao ciclo de vida de modelos de aprendizado de máquina, respectivamente.

#### O que é DataOps?

Ou **Data Operations** para os mais íntimos! 😄

É a prática de aplicar princípios de DevOps ao gerenciamento e operação de dados, com o objetivo de melhorar a qualidade, a velocidade e a eficiência do ciclo de vida dos dados.

Na comunidade, acabou se estabelencendo alguns princípios para o DataOps, como:

- **Satisfação contínua do cliente** através da entrega rápida e contínua de dados de alta qualidade.
- **Foco em análises relevantes** para impulsionar a tomada de decisões.
- **Redução de heroísmo** e dependência de indivíduos específicos, promovendo a colaboração e o trabalho em equipe.
- **Monitoramento** contínuo dos processos de dados para identificar e resolver problemas rapidamente.
- **Melhorar o cycle time** de entrega de dados, desde a coleta até a disponibilização para análise.

##### Que diacho isso tem a ver com DevOps?

Bom, vão existir diversas similaridades, desde o uso de metodologias ágeis aplicadas no desenvolvimento, até entregas contínuas que agilizam o processo de percepção de valor.

Ok, mas e ai? Quais as diferenças?

Bom, enquanto o DevOps foca na entrega de software, o DataOps foca na entrega de dados. Isso significa que o DataOps envolve práticas específicas para garantir a qualidade, a governança e a segurança dos dados ao longo de todo o ciclo de vida dos dados.

##### Mas, por qual motivo é imporatnte ter uma cultura de DataOps?

Ter uma cultura de DataOps é importante porque promove uma abordagem sistemática e colaborativa para o gerenciamento de dados, resultando em diversos benefícios, como:

- **Processos mais ágeis** e eficientes, permitindo uma entrega contínua de dados de alta qualidade.
- **Democratização do acesso aos dados**, permitindo que mais pessoas na organização possam utilizar e analisar os dados de forma independente.

##### Vamos ver algo prático?

Que tal detectarmos _data drift_ em um dataset?

> [!NOTE] 🧑🏽‍💻
> Data drift é quando a distribuição dos dados muda ao longo do tempo, o que pode afetar a performance dos modelos de machine learning. Detectar isso é crucial para manter a eficácia dos modelos.

<!-- markdownlint-disable MD033 -->
<div style="text-align:center;">
  <img src="https://docs.deepchecks.com/stable/_images/types-of-drift.png" alt="Tipos de Drift" />
  <p><i>Fonte: <a href="https://docs.deepchecks.com/stable/guides/detecting_drift.html">Deepchecks</a></i></p>
</div>

###### Qual a diferença entre os tipos de drift?

- **Concept Drift**: Mudança na relação entre as variáveis de entrada e a variável alvo ao longo do tempo.
- **Data Drift**: Mudança na distribuição das variáveis de entrada ao longo do tempo.

Resolveriamos isso, da seguinte forma, no data drift poderiamos somente atualizar o modelo, já no concept drift, teriamos que reavaliar todo o modelo.

###### Como detectar data drift?

- Monitorar dados usados para treinar o modelo.
- Atualizar o modelo regularmente com novos dados.
- Se o Concept Drift for grande, o modelo deve ser re-feito.

Mas, e ai? O que achou desse conceito de DataOps? Interessante, né?

Agora, vamos falar sobre MLOps!

#### O que é MLOps?

Ou **Machine Learning Operations** para os mais íntimos! 😄

##### Princípios do MLOps

#### Tipos de profisionais na área de dados
