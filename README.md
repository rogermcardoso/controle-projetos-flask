# 📊 Controle de Projetos - Flask App

Este é um sistema web simples para controle de projetos, desenvolvido com **Flask**, **SQLite**, **Bootstrap** e exportação para **Excel**.

## ✅ Funcionalidades

- Cadastro de projetos com campos personalizados
- Edição e exclusão de projetos
- Filtro por status ou intervalo de datas
- Exportação da base de dados para Excel (.xlsx)
- Interface responsiva com Bootstrap 5

## 🧱 Estrutura do Projeto

```
.
├── templates/ # Arquivos HTML (Jinja2 + Bootstrap)
│   ├── layout.html   
│   ├── index.html
│   ├── add_project.html 
│   └── projetos.db # Banco de dados SQLite (gerado automaticamente)
├── app.py # Arquivo principal da aplicação
├── models.py # Modelos de banco de dados 
├── export.py # Função de exportação para Excel
├── requirements.txt # Dependências 
└── README.md
```

## 📦 Requisitos

- Python 3.9+
- pip (gerenciador de pacotes)

## 📥 Instalação

Clone o projeto e instale os pacotes:

```bash
git clone https://github.com/seu-usuario/controle-projetos.git
cd controle-projetos
pip install -r requirements.txt
```


## ▶️ Como rodar
Execute o app com:

```bash
python app.py
```
Acesse no navegador:

```
http://127.0.0.1:5000/
```

## 📤 Exportação para Excel
Você pode exportar todos os projetos cadastrados clicando no botão "Exportar Excel" na página inicial. Um arquivo .xlsx será gerado para download.


## 📌 Regras de Status (automático)
O campo Status é preenchido automaticamente com base nos seguintes critérios:

- Se etapa = Paralizado → Paralizado

- Se etapa = Cancelado → Cancelado

- Se progresso = 100% → Implementado

- Caso contrário → Em andamento

## 💡 Tecnologias Usadas
- Flask
- Flask SQLAlchemy
- Bootstrap 5
- Pandas + Openpyxl

## 📁 Licença
Este projeto está licenciado sob a MIT License.
