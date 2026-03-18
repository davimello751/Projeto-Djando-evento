Etapa 1 – Conceitos Importantes

1) Por que o arquivo `.env` não deve ser versionado?

O arquivo `.env` contém informações sensíveis do projeto, como chaves secretas, senhas e configurações privadas.
Se ele for enviado para o repositório, qualquer pessoa com acesso poderá visualizar esses dados, comprometendo a segurança da aplicação.
Por isso, ele deve ser ignorado pelo `.gitignore`.

---

2) Qual a função do `pip freeze` no desenvolvimento em equipe?

O comando `pip freeze` gera uma lista de todas as dependências do projeto com suas versões exatas, geralmente salva no arquivo `requirements.txt`.
Isso permite que outros desenvolvedores instalem exatamente as mesmas bibliotecas, garantindo que o projeto funcione da mesma forma em diferentes máquinas.

---

3) O que pode acontecer se a `SECRET_KEY` for exposta?

A `SECRET_KEY` é usada pelo Django para garantir a segurança da aplicação, como na criptografia de sessões e validação de dados.
Se ela for exposta, um invasor pode:

- falsificar sessões de usuários
- acessar dados protegidos
- comprometer a segurança geral da aplicação

---

4) Qual o papel do `.gitignore` em projetos colaborativos?

O `.gitignore` define quais arquivos e pastas não devem ser enviados para o repositório.
Ele é essencial para evitar o envio de arquivos desnecessários (como cache e ambiente virtual) e arquivos sensíveis (como `.env`).
Isso mantém o repositório limpo, seguro e organizado para todos os membros da equipe.
