# API REST de Usuários - Django Rest Framework

API RESTful desenvolvida em Python com Django e Django Rest Framework para cadastro e consulta de usuários em formato JSON.

## Tecnologias utilizadas

* Python
* Django
* Django Rest Framework
* SQLite

## Como executar o projeto localmente

1. Clone este repositório e acesse a pasta do projeto:
```bash
git clone https://github.com/Adryan-Inacio/EA3-Cesmac.git
cd myapp
```

2. Crie e ative um ambiente virtual:
```bash
python -m venv venv
venv\Scripts\activate
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

4. Aplique as migrações do banco de dados:
```bash
python manage.py migrate
```

5. Crie um usuário administrador para acessar o painel de cadastro ou use o que eu já criei, username: `admin` e senha: `cesmac123`:
```bash
python manage.py createsuperuser
```

6. Inicie o servidor de desenvolvimento:
```bash
python manage.py runserver
```

## Rotas disponíveis

* **Retorno direto em JSON:** `http://127.0.0.1:8000/usuarios/?format=json`
* **Listar / Cadastrar usuários:** `GET` e `POST` em `http://127.0.0.1:8000/usuarios/`
* **Consultar / Atualizar / Remover usuário:** `GET`, `PUT` e `DELETE` em `http://127.0.0.1:8000/usuarios/{id}/`
* **Painel Administrativo:** `http://127.0.0.1:8000/admin/`