# inciar server.json =>
yarn json-server --host 192.168.0.19 server.json -p 3333

# inciar front mobile =>
- acertar baseURL: 'http://192.168.0.19:3333' ou baseURL: 'http://localhost:3333',
yarn android


# Exemplo
# Recuperação de senha

**RF** requisitos funcionais

- O usuário deve poder recuperar sua senha informando o e-mail;
- O usuário deve poder receber um email com instruções de recuperação de senha;
- O usuário deve poder resetar sua senha;

**RNF** req. não funcionais

- Utilizar o mailtrap para testar envios em ambiente de dev;
- utilizar Amazon SES para envios em produção;
- O envio de e-mails deve acontecer em segundo plano (background job);

**RN** regras de negócios

- O link enviado por email para resetar senha, deve expirar em 2h;
- O usuário precisa confirmar a nova senha ao resetar sua senha;

