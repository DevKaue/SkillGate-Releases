# SkillGate 0.2.0-preview.1

Esta versão remodela o SkillGate como uma ferramenta determinística. A IA pode criar ou corrigir uma skill, mas não participa da decisão de validação.

## Incluído

- aplicativo local aberto no navegador, com processamento em `127.0.0.1`;
- seleção direta da pasta da skill, sem prompt de tarefa e sem escolha de modelo;
- 13 regras versionadas para pacote, metadados, referências, caminhos, segredos e scripts;
- decisões `valid`, `review` e `invalid`, sem nota subjetiva;
- CLI com saída humana ou JSON;
- MCP local com `inspect_skill`, `validate_skill`, `get_rules` e `explain_rule`;
- ZIP para Windows x64 e `.deb`, AppImage e `.tar.gz` para Linux x64;
- hashes SHA-256 para os quatro artefatos.

## Verificações

- build .NET sem erros ou avisos;
- sete testes do motor determinístico;
- smoke test das quatro ferramentas MCP;
- nove testes da landing, motor no navegador e pacotes;
- teste ponta a ponta em desktop e mobile com uma skill real;
- validação estrutural do pacote Debian, AppImage e checksums.

## Limites conhecidos

- binários ainda não assinados;
- sem atualização automática ou SBOM;
- as regras verificam fatos do pacote, não garantem o comportamento futuro de um modelo.
