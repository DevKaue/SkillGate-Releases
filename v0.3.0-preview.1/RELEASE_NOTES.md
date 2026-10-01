# SkillGate 0.3.0-preview.1

## Novidades

- Editor local com as 13 regras padrão: ativação, desativação e severidade configurável.
- Até 100 regras personalizadas para arquivo obrigatório, trecho obrigatório ou trecho proibido.
- Perfil de avaliação persistido localmente, com importação, exportação e restauração do padrão.
- Limites ajustáveis de arquivos e tamanho, dentro dos limites operacionais de segurança.
- Relatórios em PDF, Markdown e JSON com gráfico de cobertura, evidências e orientações de correção.
- Identificação explícita de regras aprovadas, com falha, desativadas e não avaliadas.
- Registro do perfil utilizado, hashes do pacote e do perfil e versão do motor em cada relatório.
- CLI e MCP usam o mesmo perfil de regras do aplicativo.
- Correção de transporte UTF-8 entre o desktop e o motor no Windows.

## Atualização

Windows e AppImage continuam no canal de atualização automática assinado, com a mesma chave pública das versões anteriores. O pacote `.deb` é atualizado pela instalação da nova versão. Perfis ficam na pasta de dados locais e não são substituídos pelo instalador.

Versões antigas sem atualizador precisam instalar o novo pacote uma vez. A validação e os relatórios funcionam offline; somente a verificação e o download de atualizações usam a rede.

## Limites e segurança

As regras são determinísticas e não executam scripts ou IA. O editor configura verificações objetivas; não garante que um modelo seguirá a skill ou que o conteúdo estará livre de todos os riscos.

Esta é uma preview. A assinatura do atualizador verifica a integridade dos pacotes Windows e AppImage, mas não equivale a Authenticode do Windows. Não há certificação completa de instalação, upgrade e rollback em todas as distribuições Linux.

Motor: rule set 3.0.0, schema de relatório 3.0. Testes de motor, relatórios, fluxo de interface com o motor real e inspeção visual do PDF executados antes da publicação.
