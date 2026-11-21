# TRIDENTE — repositório relacionado (segunda ordem)

**Repositório:** Federal-Trading-ORG/company. **Papel:** Índice de empresas × APIs, organizador e consumidor de SSOT. **Data-base:** 20/11/2026 UTC. **Estado:** navegação, NÃO deploy.

## Relação e autoridade

- [Mapa canônico inter-repositórios](https://github.com/Federal-Trading-ORG/arch/blob/docs/tridente-cross-repo-index-20261120/docs/coordination/TRIDENTE_REPOSITORY_DEPENDENCIES_20261120.md).
- [Control Tower #1707](https://github.com/Federal-Trading-ORG/federaltrading.org/issues/1707) e [monorepo operacional](https://github.com/Federal-Trading-ORG/federaltrading.org).
- Manter íntegros os contratos, README, histórico, Gate 0 e boundaries existentes. CT108 mantém autoridade de sessão/membership e CT401 é autoridade de datasets próprios, sempre sujeitos a fingerprint.

## Estado e risco

O README diz que não é runtime; contratos em contracts/companies e APIs não podem fornecer um grant CT108 automaticamente. status_ops_gov em #1744 está só em draft e não pode autorizar operação baseada em rótulo de company.

## Tarefas futuras

1. Identificar branch/base SHA e ler fontes existentes, sem reinterpretar documentação histórica como runtime.
2. Obter readback independente do serviço/dados associado, com owner, UTC, source_sha, runtime_sha e served_sha.
3. Testar alternativas em staging, preservar rollback, abrir PR de implementação por owner; não efetuar deploy, DNS, autenticação ou DML só por este guia.
4. Atualizar issue existente e o mapa arch; classificação de incidente deve distinguir source fix de resultado observado.

## Rastreamento

- [#1745](https://github.com/Federal-Trading-ORG/federaltrading.org/issues/1745)
- [#1705](https://github.com/Federal-Trading-ORG/federaltrading.org/issues/1705)
- [#1478](https://github.com/Federal-Trading-ORG/federaltrading.org/issues/1478)

**Evidências mínimas:** owner, observed_at_utc, source/runtime/served digest, authority, first_failed_gate, testes realmente executados e rollback_ref. Não expor tokens, senha, cookies, HAR bruto, CNPJ de clientes ou env real.
