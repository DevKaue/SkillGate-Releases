# SkillGate Releases

Este repositorio recebera somente artefatos publicos de release, manifestos, hashes, assinaturas, SBOMs e notas. Codigo-fonte, credenciais, arquivos de projeto e dados de usuarios nao pertencem aqui.

Nenhum download deve ser publicado antes de passar pelo processo descrito em `RELEASE_POLICY.md`.

## Canais

- `preview`: pacotes portateis para avaliacao, sempre marcados quando ainda nao forem assinados;
- `stable`: somente artefatos assinados, com SBOM, proveniencia e testes completos de instalacao.

`releases.json` e a fonte legivel por maquina usada pela landing page. Cada entrada declara plataforma, tamanho, SHA-256 e estado de assinatura.

## Preview atual

`v0.2.0-preview.4` entrega um instalador NSIS assinado para o atualizador do Windows x64. O executável usa o subsistema gráfico do Windows, abre somente a janela do SkillGate e consulta automaticamente este canal público.

Os pacotes Linux da `v0.2.0-preview.2` continuam disponíveis para CLI e MCP. O pipeline do repositório privado já prepara AppImage e `.deb` assinados; o desktop Linux entrará no canal depois da primeira execução bem-sucedida desse runner.

## Canal de atualização

Este repositório é o destino público do pipeline do repositório privado SkillGate. Cada release desktop assinada publica instaladores, assinaturas e `latest.json`. O aplicativo consulta `releases/latest/download/latest.json` e só instala pacotes cuja assinatura corresponda à chave pública incorporada.

Nenhuma chave privada, token de publicação ou código-fonte privado deve ser armazenado aqui.
