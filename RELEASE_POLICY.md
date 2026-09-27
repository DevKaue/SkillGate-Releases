# Politica de release

## Go/no-go estavel

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

## Canal preview

Uma preview pode ser publicada sem assinatura, SBOM e instalador quando:

- o canal e a ausencia de assinatura estiverem visiveis antes do download;
- compilacao, testes unitarios, teste de CLI e smoke test MCP tiverem passado;
- cada pacote tiver SHA-256 publicado e instrucoes de uso;
- nenhum secret, credencial ou dado de usuario fizer parte do artefato;
- o manifesto registrar explicitamente `signed: false`.

Uma preview nunca e promovida automaticamente para `stable`.
