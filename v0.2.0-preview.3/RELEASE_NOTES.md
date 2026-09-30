# SkillGate 0.2.0-preview.3

Esta versão troca a antiga interface aberta no navegador por um aplicativo desktop real, seguindo a arquitetura do BuildArch.

## Incluído

- janela própria com Tauri 2;
- instalador NSIS `.exe` para Windows 10 e 11 x64;
- seletor nativo de pasta;
- motor determinístico .NET incorporado ao aplicativo;
- guia de uso completo dentro da ferramenta;
- preparação local de CLI e MCP para Codex e Claude;
- exportação de relatório JSON pelo diálogo nativo;
- CSP restritivo e nenhuma conexão externa.

## Depois do download

1. Execute o instalador.
2. Abra o SkillGate pelo menu Iniciar.
3. Escolha a pasta que contém `SKILL.md`.
4. Consulte erros e avisos na própria janela.
5. Exporte o relatório ou prepare a integração MCP quando necessário.

O aplicativo não abre uma URL, não depende do navegador e não inicia servidor em `localhost`.

## Verificações

- build .NET sem erros ou avisos;
- sete testes do motor determinístico;
- smoke test MCP com quatro ferramentas;
- dois testes de contrato do desktop;
- dez testes da landing, pacotes e checksums;
- inspeção das quatro áreas da interface;
- console da interface sem erros ou avisos;
- instalador conferido como executável PE/NSIS.
- instalação limpa, abertura da janela, versão do motor e desinstalação validadas em pasta isolada.

## Limites conhecidos

- instalador ainda sem assinatura de código, portanto o Windows SmartScreen pode exibir aviso;
- a versão desktop Linux ainda precisa ser construída e validada em runner Linux;
- sem atualização automática ou SBOM nesta preview.
