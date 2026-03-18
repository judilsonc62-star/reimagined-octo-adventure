# DJ Digital Center - Sistema de Gestão de Vendas

Um aplicativo completo para gerenciar vendas, estoque e estatísticas de vendas do cyber DJ Digital Center.

## 🎯 Funcionalidades

- 📊 **Dashboard** - Visão geral das vendas em tempo real
- 📦 **Gestão de Estoque** - Controlar produtos e quantidades
- 💰 **Registro de Vendas** - Registrar vendas diárias
- 📈 **Relatórios** - Estatísticas por dia, semana, mês
- 👥 **Gestão de Usuários** - Controle de acesso
- 🔧 **Configurações** - Dados da empresa

## 🛠️ Tecnologias

- **Backend**: Python + Django
- **Frontend**: HTML5 + CSS3 + JavaScript + Bootstrap
- **Banco de Dados**: SQLite
- **Servidor**: Django Development Server

## 📋 Requisitos

- Python 3.8+
- pip (gerenciador de pacotes Python)
- Navegador moderno

## ⚙️ Instalação

### 1. Clone o repositório
```bash
git clone https://github.com/judilsonc62-star/reimagined-octo-adventure.git
cd reimagined-octo-adventure
```

### 2. Crie um ambiente virtual
```bash
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
```

### 3. Instale as dependências
```bash
pip install -r requirements.txt
```

### 4. Execute as migrações do banco de dados
```bash
python manage.py migrate
```

### 5. Crie um superusuário (admin)
```bash
python manage.py createsuperuser
```

### 6. Inicie o servidor
```bash
python manage.py runserver
```

Acesse: http://127.0.0.1:8000

## 📁 Estrutura do Projeto

```
dj-digital-center/
├── manage.py
├── requirements.txt
├── db.sqlite3
├── dj_digital_center/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── vendas/
│   ├── migrations/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── forms.py
│   └── templates/
├── estoque/
│   ├── migrations/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── forms.py
│   └── templates/
├── relatorios/
│   ├── migrations/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── templates/
├── usuarios/
│   ├── migrations/
│   ├── models.py
│   ├── views.py
��   ├── urls.py
│   ├── forms.py
│   └── templates/
└── static/
    ├── css/
    ├── js/
    └── images/
```

## 🚀 Como Usar

### 1. Acessar a Dashboard
- URL: `http://localhost:8000/dashboard`
- Faça login com suas credenciais

### 2. Gerenciar Estoque
- URL: `http://localhost:8000/estoque/produtos`
- Adicione, edite ou remova produtos

### 3. Registrar Vendas
- URL: `http://localhost:8000/vendas/nova`
- Registre as vendas do dia

### 4. Ver Relatórios
- URL: `http://localhost:8000/relatorios/`
- Consulte estatísticas por período

## 📊 Modelos de Dados

### Produto
- ID
- Nome
- Descrição
- Preço de custo
- Preço de venda
- Quantidade em estoque
- Data de adição

### Venda
- ID
- Produto
- Quantidade vendida
- Preço unitário
- Total
- Data da venda
- Usuário que fez a venda

### Usuário
- ID
- Nome
- Email
- Senha
- Perfil (admin, vendedor)
- Ativo/Inativo

## 👨‍💻 Autor

Desenvolvido para DJ Digital Center

## 📝 Licença

MIT License