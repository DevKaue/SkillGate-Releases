# SkillGate 0.1.0-preview.1

Primeira preview publica do motor local de validacao.

## Incluido

- sete gates determinísticos: estrutura, escopo, contrato, cobertura, atualidade, seguranca e compatibilidade;
- relatorio JSON com decisao, score, findings, digest SHA-256 e identificador reproduzivel;
- CLI para validacao de `SKILL.md`;
- servidor MCP por stdio com `validate_skill`, `get_policy` e `explain_finding`;
- binarios autossuficientes para Windows x64 e Linux x64.

## Limites conhecidos

- binarios ainda nao assinados;
- sem interface desktop, atualizacao automatica, SBOM ou adapters semanticos de IA;
- a ferramenta valida o contrato, mas nao executa a skill.
