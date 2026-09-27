# SkillGate 0.1.0-preview.2

Esta preview amplia a distribuicao Linux para oferecer as mesmas opcoes de instalacao encontradas na pagina de referencia.

## Incluido

- pacote `.deb` para Debian, Ubuntu e distribuicoes derivadas;
- AppImage tipo 2 para outras distribuicoes Linux x86_64;
- pacote portatil `.tar.gz` mantido para instalacoes manuais;
- pacote portatil `.zip` para Windows x64;
- CLI local e servidor MCP por stdio com `validate_skill`, `get_policy` e `explain_finding`;
- hashes SHA-256 de todos os quatro artefatos.

## Verificacoes

- build .NET sem avisos ou erros;
- quatro testes do motor de politicas;
- smoke test MCP;
- validacao estrutural do pacote Debian e do AppImage;
- validacao dos hashes publicados.

## Limites conhecidos

- binarios ainda nao assinados;
- sem interface desktop, atualizacao automatica ou SBOM;
- a ferramenta valida o contrato, mas nao executa a skill.
