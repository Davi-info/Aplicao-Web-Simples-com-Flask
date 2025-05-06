Protótipo Funcional de uma Aplicação Web Simples com Flask

# Descrição do Projeto
O ShoPI é um sistema de gerenciamento para pequenos comércios, desenvolvido em Flask (Python), que permite o cadastro e gerenciamento de clientes e produtos. O sistema oferece uma interface web intuitiva para realizar operações CRUD (Create, Read, Update, Delete) sobre esses dados.

# Funcionalidades Implementadas

### 👥 Módulo de Clientes
- **Cadastro Completo**:
  - Nome completo (apenas letras e espaços)
  - E-mail válido (com validação de formato)
  - Data de nascimento
  - Cidade (apenas letras e espaços)
  - Telefone
- **Listagem Organizada de clientes**:
  - Tabela responsiva com todos os campos
  - Ordenação por ID
- **Edição Segura**:
  - Mesmas validações do cadastro
  - Persistência imediata no banco
- **Exclusão com Confirmação**:
  - Modal de confirmação
  - Feedback visual

# 📦 Módulo de Produtos
Cadastro de produtos: Inclusão de novos produtos com nome, preço, estoque, quantidade, marca e categoria

Listagem de produtos: Visualização de todos os produtos cadastrados em formato de tabela

Edição de produtos: Atualização dos dados dos produtos existentes

Exclusão de produtos: Remoção de produtos do sistema

# Outras Funcionalidades
- Validação de campos obrigatórios e formatos de entrada (e.g., e-mail, números).
- Mensagens de feedback para o usuário (sucesso ou erro).
- Interface estilizada com CSS para uma melhor experiência do usuário.

## Estrutura do Projeto
```
ShoPI/
├── app/
│   └── controller.py # Lógica de controle (rotas e validações)			
│   └── model.py # Modelos de dados (Clientes e Produtos)            
│   └── view.py # Configuração das rotas da aplicação            
│   └── instance/

├── static/
│   └── css/                # Arquivos de estilo CSS

├── Templates/              # Templates HTML para renderização 

├── venv/ # Armazena o ambiente virtual do Python, isolando as dependências do projeto para evitar conflitos com outras aplicações

├── db.py # Configuração do SQLAlchemy	
             
├── main.py  # Arquivo principal para execução do projeto
│  	
└── README.md  # Documentação do projeto
```

# Tecnologias Utilizadas 
Backend: Python com Flask

Banco de Dados: SQLite

Frontend: HTML5, CSS3

ORM: SQLAlchemy


# Passos para Execução

Pré-requisitos:
Python 3.7 ou superior instalado, Pip (gerenciador de pacotes do Python)

Clone o repositório (se aplicável) ou copie os arquivos do projeto para uma pasta local

# Crie um ambiente virtual (recomendado):

python -m venv venv

# Ative o ambiente virtual:

# No Windows:

venv\Scripts\activate

# No Linux/MacOS:

source venv/bin/activate

# Instale as dependências:

pip install flask flask-sqlalchemy

# No terminal Python após executar flask shell
db.create_all()

# Execute a aplicação:

python main.py

# Acesse a aplicação:
Abra seu navegador e acesse:

http://127.0.0.1:5000

# Primeiros Passos
Ao acessar a aplicação, você verá a página inicial com opções para:

Cadastrar novo produto

Cadastrar novo cliente

Visualizar produtos cadastrados

Visualizar clientes cadastrados

Utilize os menus de navegação para acessar as diferentes funcionalidades do sistema
