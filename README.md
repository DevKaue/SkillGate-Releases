# SkillGate Releases

Este repositorio recebera somente artefatos publicos de release, manifestos, hashes, assinaturas, SBOMs e notas. Codigo-fonte, credenciais, arquivos de projeto e dados de usuarios nao pertencem aqui.

Nenhum download deve ser publicado antes de passar pelo processo descrito em `RELEASE_POLICY.md`.

## Canais

- `preview`: pacotes portateis para avaliacao, sempre marcados quando ainda nao forem assinados;
- `stable`: somente artefatos assinados, com SBOM, proveniencia e testes completos de instalacao.

`releases.json` e a fonte legivel por maquina usada pela landing page. Cada entrada declara plataforma, tamanho, SHA-256 e estado de assinatura.

## Preview atual

`v0.2.0-preview.2` entrega um executável único e autossuficiente para Windows x64, sem ZIP ou instalação do .NET. A interface agora inclui as áreas Validar, Como usar e Codex e Claude. Para Linux x64 há `.deb`, AppImage e `.tar.gz`. Os binários ainda não são assinados e não devem ser tratados como release estável.
