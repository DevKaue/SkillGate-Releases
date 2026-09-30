# SkillGate Releases

Este repositorio recebera somente artefatos publicos de release, manifestos, hashes, assinaturas, SBOMs e notas. Codigo-fonte, credenciais, arquivos de projeto e dados de usuarios nao pertencem aqui.

Nenhum download deve ser publicado antes de passar pelo processo descrito em `RELEASE_POLICY.md`.

## Canais

- `preview`: pacotes portateis para avaliacao, sempre marcados quando ainda nao forem assinados;
- `stable`: somente artefatos assinados, com SBOM, proveniencia e testes completos de instalacao.

`releases.json` e a fonte legivel por maquina usada pela landing page. Cada entrada declara plataforma, tamanho, SHA-256 e estado de assinatura.

## Preview atual

`v0.2.0-preview.1` transforma o SkillGate em uma ferramenta local completa: aplicativo no navegador local, CLI e servidor MCP usando o mesmo motor determinístico. A decisão não usa IA, tarefa ou perfil de executor. Há ZIP para Windows x64 e `.deb`, AppImage e `.tar.gz` para Linux x64. Os binários ainda não são assinados e não devem ser tratados como release estável.
