# 📊 Controle de Projetos - Flask App

Este é um sistema web simples para controle de projetos, desenvolvido com **Flask**, **SQLite**, **Bootstrap** e exportação para **Excel**.

## ✅ Funcionalidades

- Cadastro de projetos com campos personalizados
- Edição e exclusão de projetos
- Filtro por status ou intervalo de datas
- Exportação da base de dados para Excel (.xlsx)
- Interface responsiva com Bootstrap 5

## 🧱 Estrutura do Projeto

controle_projetos/ │ ├── app.py # Arquivo principal da aplicação ├── models.py # Modelos de banco de dados ├── export.py # Função de exportação para Excel ├── requirements.txt # Dependências │ ├── templates/ # Arquivos HTML (Jinja2 + Bootstrap) │ ├── layout.html │ ├── index.html │ └── add_project.html │ └── projetos.db # Banco de dados SQLite (gerado automaticamente)

## 📦 Requisitos

- Python 3.9+
- pip (gerenciador de pacotes)

## 📥 Instalação

Clone o projeto e instale os pacotes:

```bash
git clone https://github.com/seu-usuario/controle-projetos.git
cd controle-projetos
pip install -r requirements.txt
