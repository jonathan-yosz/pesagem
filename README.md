# ♻️ Pesagem de Recicláveis

> **Projeto criado com o [Claude](https://claude.ai), da Anthropic.**

App para celular que substitui o caderno na pesagem de materiais recicláveis. Cada cliente tem seus próprios materiais e preços por quilo, e no final o app gera uma imagem PNG com a tabela de pesos e valores.

## Funções

- **Clientes fixos:** cada cliente tem seus próprios materiais, com preço por kg próprio. Configure uma vez e ajuste quando precisar.
- **Tabela estilo planilha:** cada material é uma coluna, com quantas pesagens forem necessárias (ex.: 45 + 55 + 30 = 130 kg).
- **Cálculo automático:** total de peso, `x preço por kg` e total em dinheiro de cada material, mais o total geral do cliente.
- **Modo unidades (`und`):** lance a quantidade e o peso de cada unidade (ex.: 22 und × 1,35 kg). Dá para misturar kg e unidades no mesmo material.
- **Modo desconto (`desc`):** o peso lançado é descontado do total do material, como o de uma caixa ou de um saco. Funciona em kg ou em unidades.
- **Data:** volta para o dia de hoje ao iniciar uma nova pesagem, e pode ser alterada à mão.
- **Exportar PNG:** imagem em branco e verde com preços, pesagens, totais, data e nome do cliente, pronta para salvar ou enviar.
- **Backup e restauração:** salva e restaura clientes, materiais e preços em um arquivo.
- **Funciona offline:** depois de instalado, não precisa de internet.

## Como usar

1. Abra o endereço do app no Chrome do celular.
2. Toque nos três pontinhos e escolha **Instalar app** (ou **Adicionar à tela inicial**).
3. Na aba **Clientes**, cadastre o cliente, os materiais e o preço por kg de cada um.
4. Na aba **Pesagem**, escolha o cliente, digite o peso e toque em **+**.
5. Ao terminar, toque em **Exportar PNG**. Para a próxima pesagem, toque em **Nova pesagem**.

## Privacidade

Clientes, preços e pesagens ficam guardados **somente no navegador do seu aparelho**. Nada é enviado para servidores. Use **Salvar backup** de vez em quando para não perder os dados ao trocar de celular ou limpar o navegador.

## Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | O aplicativo completo (página, estilo e lógica) |
| `manifest.webmanifest` | Dados para instalar como app |
| `sw.js` | Faz o app funcionar offline e receber atualizações |
| `icon-*.png` | Ícones do app |
