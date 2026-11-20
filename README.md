# Prometheus-Sys-ORG / company

Repositório **organizador** para SSOT **prometheus-sys.org** no eixo **empresas × APIs** (plano de controlo e consumo por suites).

- **Não** é runtime canónico de aplicações aqui.
- **Não** armazenar credenciais nem `.env` reais (ver `.gitignore`).
- **Consumo suite canónico:** `Federal-Trading-ORG/federaltrading.org` (`contracts/suite-consumer/`, `manifests/migration/`).

## Árvore

| Caminho | Função |
|---------|--------|
| `contracts/ssot/` | Locks de superfície |
| `contracts/apis/` | Catálogo lógico CT142/144/145 |
| `contracts/companies/` | Empresa → superfícies |
| `manifests/migration/` | Vista PS alinhada ao manifest FT |
| `docs/` | Pontes e convenções |


## TRIDENTE — índice de integração (20/11/2026)

- [Papel, dependências e gates do repositório](docs/tridente/INTEGRATION_STATUS_20261120.md).
- [Mapa de primeira/segunda ordem e precedência](https://github.com/Federal-Trading-ORG/arch/blob/docs/tridente-cross-repo-index-20261120/docs/coordination/TRIDENTE_REPOSITORY_DEPENDENCIES_20261120.md). Informação complementar: README e políticas anteriores permanecem inalterados.
