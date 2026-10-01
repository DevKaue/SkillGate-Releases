# SkillGate 0.2.0-preview.4

## Alterações

- remove a janela de terminal no Windows;
- verifica atualizações automaticamente ao iniciar e a cada seis horas;
- permite verificar manualmente pela barra lateral;
- baixa e instala atualizações assinadas pelo canal público oficial;
- mantém a chave privada somente nos Secrets do repositório privado;
- adiciona pipeline preparado para Windows e Linux.

## Segurança

O aplicativo só aceita pacotes compatíveis com a chave pública incorporada. Alterar `latest.json`, o instalador ou a assinatura não permite instalar um pacote adulterado.
