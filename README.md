Etapa 1 – Respostas

1. Por que o arquivo .env não deve ser versionado?
O arquivo .env contém informações sensíveis do projeto, como senhas, chaves de API e a SECRET_KEY do Django.
Se ele for versionado (enviado para o GitHub), essas informações podem ser expostas publicamente, colocando a segurança da aplicação em risco.
Por isso, ele deve ser incluído no .gitignore.

2. Qual a função do pip freeze no contexto de desenvolvimento em equipe?
O comando pip freeze serve para listar todas as dependências do projeto com suas versões exatas.
Isso permite gerar o arquivo requirements.txt, garantindo que todos os membros da equipe instalem exatamente as mesmas bibliotecas,
evitando erros e incompatibilidades.

3. O que pode acontecer se a SECRET_KEY for exposta?
Se a SECRET_KEY for exposta, um invasor pode comprometer a segurança da aplicação.
Ele pode, por exemplo, falsificar sessões de usuários, gerar tokens inválidos,
acessar dados protegidos ou até executar ações maliciosas dentro do sistema.
Isso pode levar à perda de dados e quebra da segurança da aplicação.

4. Qual o papel do .gitignore em projetos colaborativos?
O .gitignore define quais arquivos e pastas não devem ser enviados para o repositório.
Em projetos colaborativos, ele evita o versionamento de arquivos desnecessários ou sensíveis, como o .env,
arquivos temporários, cache e o ambiente virtual (venv).
Isso mantém o repositório organizado, seguro e mais leve para toda a equipe.
