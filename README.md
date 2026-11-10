# BRAGA Consulta Veicular

## Versão 1.9.46 — 10/11/2026

Atualize pelo botão **Verificar atualizações** no BRAGA.

[Instalador e notas da versão 1.9.46](https://github.com/guicbragadesp/consulta-veicular-sp/releases/tag/v1.9.46)

- Inclui Restrição RENAVE (Confirmado Estoque) e Comunicação RENAVE (Saída Estoque).
- RENAVE com “Não informado” não gera alerta. Resultados que exigem atenção aparecem em vermelho e negrito, com o mesmo aviso das outras restrições.
- Mostra “POSSÍVEL DÉBITO DE DÍVIDA ATIVA” quando há IPVA devido e pagamento efetuado zerado. Nessa situação, exige consulta direta à PGE mesmo com “Nada consta” na Fazenda.
- Preserva o “Nada consta” retornado pela própria PGE e não soma o IPVA devido como dívida automaticamente.

Validação: 34 testes passaram; instalação conferida com backup e preservação dos dados. Feche e reabra o BRAGA após instalar.

## Correção da emissão de guias da PGE para o BRAGA 1.9.44

O fluxo de emissão aceita os botões Gerar DARE e Download DARE da PGE e tenta fechar o aviso Importante antes de baixar a guia. A correção também aceita os rótulos GARE.

[Baixar a correção manual da PGE para a versão 1.9.44](atualizacoes/BRAGA-1.9.44-correcao-emissao-PGE.zip)

Com o BRAGA 1.9.44 fechado, extraia o ZIP e copie o arquivo da pasta `app` extraída para a pasta `app` do programa, substituindo `pge-guides.js`. Reabra o BRAGA após copiar o arquivo.

## Versão 1.9.30 — 02/10/2026

Inclui a versão 1.9.29 de 01/10 e a correção do Detran de 02/10.

**Atualize pelo botão Verificar atualizações no Braga.**

[Instalador e notas da versão 1.9.30](https://github.com/guicbragadesp/consulta-veicular-sp/releases/tag/v1.9.30)

Feche o programa antes da atualização e reabra após concluir. Dados e logins são preservados, e os arquivos atuais recebem backup.

- Campos Taxa de transferência, Vistoria e Placa separados e na ordem correta.
- Total destacado no PDF e na imagem copiada, com seta verde antes do valor.
- Leitura corrigida das seis categorias de restrições do Detran.
- Alertas para intenção de gravame, demais restrições e GNV.
- Consulta do Detran opcional e correção do cadastro/seleção de login gov.br.
- Tratamento do aviso informativo da Fazenda preservado.

Validação: 50 testes automatizados passaram; sintaxe JavaScript verificada; os 33 arquivos do instalador foram extraídos e conferidos. O seletor de atualizações reconheceu a versão publicada e seu SHA-256.

Alternativa manual: [pacote ZIP](atualizacoes/BRAGA-1.9.30-atualizacao-combinada.zip). Extraia e execute Atualizar.cmd, indicando a pasta que contém app e runtime.
