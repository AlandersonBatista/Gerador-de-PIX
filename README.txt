# Gerador de Pix (PWA) — v4

Ajustes desta versão:
- Campo renomeado para "Mensagem para o recebedor (opcional)".
- Mensagem **não é salva** no navegador (sempre começa em branco).
- Sanitização em tempo real da mensagem:
  - remove acentos;
  - converte para maiúsculas;
  - permite apenas letras, números, espaço, ponto e hífen;
  - limita a 50 caracteres.
- Cidade fixa "RIO DE JANEIRO" no payload.
- Nome do recebedor fixo "RECEBEDOR".
- Txid sempre gerado automaticamente.
- Envio para WhatsApp com **apenas** o código Pix.
