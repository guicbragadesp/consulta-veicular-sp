# BRAGA Consulta Veicular

## Versão 1.9.30 — 02/10/2026

Atualização combinada: inclui a versão 1.9.29 de 01/10/2026 e a correção da leitura de restrições do Detran-SP de 02/10/2026.

[Baixar BRAGA 1.9.30](https://github.com/guicbragadesp/consulta-veicular-sp/raw/refs/heads/main/atualizacoes/BRAGA-1.9.30-atualizacao-combinada.zip)

Feche o Braga, extraia o ZIP e execute Atualizar.cmd. Informe a pasta do programa que contém app e runtime. O atualizador cria backup e preserva dados e logins. O pacote contém os arquivos do aplicativo e os testes.

### Alterações

- Preserva campos separados de Taxa de transferência, Vistoria e Placa, na ordem correta.
- Preserva destaque do total no PDF e na imagem copiada, com seta verde antes do valor.
- Preserva o tratamento do aviso informativo da Fazenda.
- Corrige a leitura das seis categorias de restrições do Detran mesmo quando os cartões ficam fora do contêiner antigo.
- Alerta para intenção de gravame, demais restrições e combustível GNV.
- Consulta do Detran permanece opcional.
- Mantém a correção do cadastro e seleção dos logins gov.br.

Validação: 50 testes automatizados passaram e sintaxe de todos os módulos JavaScript verificada. Leitura do Detran confirmada pelo usuário antes da combinação; consulta real da versão combinada permanece por confirmar.

Este ZIP é uma atualização manual para quem já tem o programa instalado. O botão Verificar atualizações continua usando os instaladores da seção Releases; esta publicação não altera esse canal.
