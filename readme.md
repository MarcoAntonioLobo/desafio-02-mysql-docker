🐳 Ambiente de Desenvolvimento com MySQL + Docker
Este projeto configura rapidamente um banco de dados MySQL para desenvolvimento usando Docker e Docker Compose.

Ideal para desenvolvedores que querem um setup rápido, padronizado e sem necessidade de instalação local do MySQL.

🚀 Objetivo
Criar um banco de dados MySQL com as seguintes configurações:
```
📛 Nome do banco: docker_db

👤 Usuário: docker_usr

🔐 Senha: docker_pwd

🧪 Ambiente: Apenas para desenvolvimento (sem persistência obrigatória dos dados)
```
🗂 Estrutura do Projeto
```bash

.
├── Dockerfile              # Imagem personalizada do MySQL
├── docker-compose.yml      # Orquestração do container
├── .env                    # Variáveis de ambiente do banco
├── .gitignore              # Ignora arquivos sensíveis e desnecessários
└── README.md               # Documentação do projeto
```
🛠 Pré-requisitos
Docker

Docker Compose

Confirme que estão instalados:

```bash

docker -v
docker-compose -v
```
⚙️ Como usar
Clone o repositório ou copie os arquivos:

```bash

git clone <url-do-seu-repo>
cd nome-do-projeto
```
Configure as variáveis no arquivo .env (se quiser alterar padrões).

Inicie o container:

```bash

docker-compose up -d
```
O container mysql_dev será criado, expondo o MySQL na porta 3306.

🧪 Testando a conexão
Use qualquer cliente MySQL (MySQL Workbench, DBeaver, CLI mysql, etc) com:
```
Campo	Valor
Host	localhost
Porta	3306
Banco de Dados	docker_db
Usuário	docker_usr
Senha	docker_pwd
```
📦 Parar ou remover o container
Para parar:

```bash

docker-compose down
```
Para parar e apagar volumes (se usados):

```bash

docker-compose down -v
```
🧾 .gitignore
Ignora arquivos sensíveis, dados locais e configurações de IDEs.

📬 Contato
```
Marco Lobo
marcoantoniolobo82@gmail.com
```