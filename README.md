# SkillGate Releases

Este repositorio recebera somente artefatos publicos de release, manifestos, hashes, assinaturas, SBOMs e notas. Codigo-fonte, credenciais, arquivos de projeto e dados de usuarios nao pertencem aqui.

Nenhum download deve ser publicado antes de passar pelo processo descrito em `RELEASE_POLICY.md`.

## Canais

- `preview`: pacotes portateis para avaliacao, sempre marcados quando ainda nao forem assinados;
- `stable`: somente artefatos assinados, com SBOM, proveniencia e testes completos de instalacao.

`releases.json` e a fonte legivel por maquina usada pela landing page. Cada entrada declara plataforma, tamanho, SHA-256 e estado de assinatura.

## Preview atual

`v0.2.0-preview.3` entrega um instalador NSIS para Windows x64 com aplicativo Tauri, janela própria e motor determinístico incorporado. Não abre navegador, não inicia servidor local e não exige instalação do .NET. A interface inclui as áreas Validar, Como usar, Codex e Claude e Sobre. Os binários ainda não são assinados e não devem ser tratados como release estável.

Os pacotes Linux da `v0.2.0-preview.2` continuam disponíveis para CLI e MCP. O desktop Tauri para Linux será publicado somente depois de ser gerado e testado em ambiente Linux.
