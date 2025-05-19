# Automação n8n - Exemplo API + E-mail

Este projeto contém um workflow criado no [n8n](https://n8n.io) que realiza as seguintes ações:

1. Dispara automaticamente todos os dias (via nó Cron).
2. Faz uma requisição HTTP para uma API pública de testes (`jsonplaceholder.typicode.com`).
3. Extrai o título da resposta.
4. Envia o resultado por e-mail.

## Pré-requisitos

- Conta gratuita no [n8n.cloud](https://n8n.cloud) ou instalação local.
- Conta de e-mail com SMTP habilitado (ex: Gmail).
- Permissão para usar senhas de aplicativos (em caso de Gmail).

## Como usar

1. Importe o arquivo `automacao-api-email.json` no seu editor do n8n:
   - Clique nos três pontos no canto superior direito do editor.
   - Vá em **Import** e selecione o arquivo.

2. Configure o nó **Send Email** com seus dados SMTP:
   - Email de envio.
   - Senha ou app password.
   - Destinatário (campo "To").

3. Teste cada nó clicando em **Execute Node**.

4. Clique em **Save** e depois **Activate** para ativar a automação.

## Resultado esperado

Você receberá um e-mail com o título da tarefa número 1 da API:



