# 🎫 TicketPass API

API REST para **emissão, gestão e validação de bilhetes digitais** (eventos e viagens),
com tokens assinados e QR Code, para reduzir fraudes e impedir a reutilização de bilhetes.

## Equipa

| Nome | Módulo principal |
|---|---|
| Araújo | Eventos/Viagens e Relatórios |
| Lesliana | Emissão de bilhetes, Token e QR Code |
| Vassa | Validação, Redis e Histórico |

## Tecnologias

Java 21+ · Spring Boot · PostgreSQL · Redis · Docker · Swagger/OpenAPI · JUnit · ZXing

## Como correr (em desenvolvimento)

1. Instalar Java, Docker e Git
2. Clonar o repositório: `git clone <URL-do-repositório>`
3. Subir a base de dados e o Redis: `docker compose up -d`
4. Arrancar a API (o projecto Spring Boot será adicionado na Fase 0)

## Estrutura do repositório

```
ticketpass-api/
├─ docs/                 Documentação do projecto (XP + Scrum)
│  ├─ 01-capitulo-2-caracteristicas-e-planificacao.md
│  ├─ 02-capitulo-3-implementacao-e-provas.md
│  ├─ anexos/            Levantamento de requisitos original
│  └─ diagramas/         Modelo de dados, cartões CRC, etc.
├─ docker-compose.yml    PostgreSQL + Redis
├─ CONTRIBUINDO.md       Regras de trabalho em equipa
└─ README.md
```

## Estado do projecto

| Fase | Descrição | Estado |
|---|---|---|
| 0 | Preparação | ⬜ Por fazer |
| 1 | Base do sistema (eventos e bilhetes simples) | ⬜ Por fazer |
| 2 | Token e QR Code | ⬜ Por fazer |
| 3 | Validação completa (**MVP**) | ⬜ Por fazer |
| 4 | Redis (concorrência) | ⬜ Por fazer |
| 5 | Relatórios e extras | ⬜ Por fazer |
| 6 | Fecho | ⬜ Por fazer |

## Documentação

Ver a pasta [`docs/`](docs/).
