# SkillGate 0.2.0-preview.2

Esta versão deixa a experiência de primeiro uso mais direta, especialmente no Windows.

## Incluído

- download direto de um único arquivo `.exe`, sem ZIP ou RAR;
- executável Windows autossuficiente, sem instalação do .NET;
- guia completo dentro do aplicativo;
- áreas separadas para Validar, Como usar e Codex e Claude;
- exemplos de CLI e configuração MCP incorporados;
- proteção de sessão nas requisições locais;
- `.deb`, AppImage e `.tar.gz` atualizados para Linux x64;
- checksums SHA-256 para todos os artefatos.

## Verificações

- execução do `.exe` fora da pasta de build e sem arquivos auxiliares;
- build .NET sem erros ou avisos;
- sete testes do motor determinístico;
- dez testes da landing, artefatos e checksums;
- teste ponta a ponta do aplicativo com guia, ajuda MCP e uma skill real;
- teste ponta a ponta do domínio de produção em desktop e mobile;
- validação estrutural do pacote Debian e AppImage.

## Limites conhecidos

- binários ainda não assinados;
- o aplicativo abre a interface local no navegador padrão;
- sem atualização automática ou SBOM.
