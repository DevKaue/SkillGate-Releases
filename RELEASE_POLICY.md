# Politica de release

## Go/no-go

Uma release exige:

- commit imutavel e tag assinada;
- build limpo em runners controlados;
- testes do core, CLI, MCP e instaladores;
- threat model e validacao de regressao atualizados;
- SBOM, proveniencia, SHA-256 e assinatura por artefato;
- instalacao limpa, upgrade, desinstalacao e rollback testados;
- notas de release com compatibilidade e migracoes;
- responsavel pelo monitoramento e mecanismo de revogacao.

## Credenciais

Chaves de assinatura e publicacao ficam em cofre de CI ou servico de assinatura. Chaves de IA dos usuarios nunca participam do build e permanecem no keychain da maquina do usuario.

## Layout de cada versao

```text
vX.Y.Z/
  manifest.json
  checksums.txt
  sbom.spdx.json
  provenance.intoto.jsonl
  windows/
  linux/
```

Artefatos nao verificados nao podem ser expostos como download na landing page.
