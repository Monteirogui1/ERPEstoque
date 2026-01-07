# ERP de Estoque – Django 🐍📊

Sistema ERP de **gestão de estoque** desenvolvido em **Django**, focado em controle de produtos, categorias, fornecedores, marcas, movimentações, lotes e métricas gerenciais, com suporte a **multiempresa (multi-cliente)**.

## 🚀 Funcionalidades Principais

### 🔐 Autenticação & Multiempresa
- Sistema de usuários por cliente
- Controle de acesso por login
- Isolamento total de dados por empresa (cliente)

### 📦 Gestão de Estoque
- Cadastro de produtos com variações
- Controle de estoque por unidade e lote
- Estoque mínimo com alertas automáticos
- Histórico completo de movimentações

### 🔄 Movimentações
- Entradas, saídas e ajustes de estoque
- Controle por lote
- Importação de Nota Fiscal (XML)
- Validação automática de saldo

### 📊 Dashboard & Métricas
- Total de vendas e entradas
- Valor de estoque (custo e venda)
- Lucro estimado
- Produtos mais e menos vendidos
- Gráficos por período (dia, semana, mês)

### 🧾 Cadastros Gerais
- Categorias
- Fornecedores
- Marcas
- Unidades de medida
- Campos dinâmicos por categoria

### 📥 Importação & Exportação
- Importação e exportação de produtos e variações
- Suporte a CSV, JSON e XLSX

### 🔔 Notificações
- Alertas de estoque mínimo
- Registro de notificações no sistema
- Envio de e-mail automático

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **Django**
- **Django ORM**
- **HTML / CSS / JavaScript**
- **Chart.js** (gráficos)
- **Django Import-Export**
- **Waitress** (produção)
- **PostgreSQL / SQLite** (compatível)

---

## ⚙️ Instalação e Execução

### 1️⃣ Clone o repositório
```bash
git clone https://github.com/seu-usuario/erp-estoque.git
cd erp-estoque

2️⃣ Crie e ative o ambiente virtual
python -m venv venv
venv\Scripts\activate  # Windows

3️⃣ Instale as dependências
pip install -r requirements.txt

4️⃣ Execute as migrações
python manage.py migrate

5️⃣ Crie um superusuário
python manage.py createsuperuser

6️⃣ Execute o projeto
python manage.py runserver


Acesse:
👉 http://127.0.0.1:8000
```

## 🏭 Produção (Windows Service)

O projeto possui suporte para execução como serviço do Windows, utilizando Waitress, via arquivo:
```
django_service.py
```

## Ideal para ambientes corporativos.

📌 Estrutura do Projeto
```
apps/
 ├── authentication
 ├── categorias
 ├── fornecedor
 ├── marcas
 ├── produtos
 ├── movimentacao
 ├── notificacao
 ├── home
 └── shared
core/
 ├── settings.py
 ├── urls.py
 └── wsgi.py
```

📄 Licença

Este projeto é de uso interno / educacional.
Sinta-se à vontade para adaptar conforme sua necessidade.
