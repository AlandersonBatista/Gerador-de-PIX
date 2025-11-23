# Gerador de Pix (PWA) — v9 com QR Code + Log + PDF + Limpar histórico

### Novidades desta versão (v9)

1. **Botão "🗑️ Limpar histórico"**
   - Apaga todos os registros salvos no log local (`pix-log-v1`).
   - Atualiza o campo de histórico para "Nenhum registro ainda.".
   - Exige confirmação (`confirm`) antes de limpar, para evitar exclusão acidental.

2. **Informação clara sobre o limite de registros**
   - Na seção de histórico foi incluído o texto:
     > "Este histórico é local deste aparelho e armazena apenas os últimos 100 Pix gerados. Use 'Limpar histórico' para começar uma nova lista quando quiser."
   - Deixa explícito para o usuário que:
     - O log é local.
     - Existe limite de **100** registros.
     - Ele pode resetar quando achar necessário.

### Funcionalidades mantidas da v8

- Geração de código Pix (copia e cola) com validações de chave (CPF, CNPJ, e-mail, telefone, aleatória).
- Geração e exibição de QR Code em tela.
- Registro automático no log local (Txid, valor, recebedor, mensagem, data/hora) a cada Pix gerado.
- Exibição do histórico em texto.
- Envio do histórico em texto via WhatsApp.
- Geração de relatório em PDF usando jsPDF.
- Download do PDF no aparelho ("Baixar relatório em PDF").
- Compartilhamento do PDF via `navigator.share` (inclusive para WhatsApp, em aparelhos compatíveis).
- Envio do código Pix sozinho pelo WhatsApp.
- Envio do QR Code + código como legenda, em navegadores/aparelhos que suportam compartilhamento com arquivos.
