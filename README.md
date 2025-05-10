# Traffic Time Analyzer

Sistema para coletar, armazenar e analisar tempos de trajeto de carro em áreas urbanas, com o objetivo de identificar padrões de tráfego com base em dados reais da Google Maps API.

## Objetivos

- Coletar dados de tempo estimado de trajeto para diferentes rotas e horários.
- Armazenar os dados em um banco relacional.
- Calcular médias de tempo de viagem.
- Exibir os dados de forma simples para análise.

## Arquitetura

O projeto é dividido em três componentes principais:

### Backend

- Linguagem: Go
- Framework: Gin
- Funções:
  - Requisições à Google Maps API.
  - Armazenamento dos dados.
  - API REST para o frontend.

### Banco de Dados

- SGBD: PostgreSQL
- Ambiente: Docker
- Uso: Armazenamento de dados de trajetos e coletas.

### Frontend

- Tecnologias: React, Tailwind CSS, Jotai
- Funções: Interface para visualização dos dados coletados.

## Containers

Utilizamos Docker para isolar os serviços:

- backend (Go)
- db (PostgreSQL)
- frontend (React)

## API de Mapas

- Fonte: Google Maps API
- Uso: Obtenção de tempo estimado com tráfego em tempo real.
