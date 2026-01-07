# 🥋 Sistema de Treino (Django + Django Ninja)

Aplicação desenvolvida em **Django** com **Django Ninja** para gerenciamento de alunos, aulas concluídas e progressão de faixas em artes marciais.

---


## Layout web
![Web 1](https://github.com/GuilhermeGTM/Api-Treino/blob/main/GitHubMidia/1.png)

![Web 1](https://github.com/GuilhermeGTM/Api-Treino/blob/main/GitHubMidia/2.png)

![Web 1](https://github.com/GuilhermeGTM/Api-Treino/blob/main/GitHubMidia/3.png)

![Web 1](https://github.com/GuilhermeGTM/Api-Treino/blob/main/GitHubMidia/4.png)

---

## 📌 Funcionalidades

- Cadastro de **alunos** com nome, email, data de nascimento e faixa atual.
- Registro de **aulas concluídas** por aluno.
- Cálculo automático de **progresso do aluno**:
  - Total de aulas concluídas na faixa atual.
  - Quantidade de aulas necessárias para avançar para a próxima faixa.
- Validação de regras de graduação:
  - Menores de 18 anos não podem receber faixas avançadas (Azul, Roxa, Marrom, Preta).
- API REST com endpoints para:
  - Criar aluno.
  - Listar alunos.
  - Consultar progresso de um aluno.
  - Registrar aulas realizadas.
  - Atualizar dados do aluno.

---

## ⚙️ Tecnologias Utilizadas

| Tecnologia          | Descrição                                                                 |
|---------------------|---------------------------------------------------------------------------|
| **Python 3.x**      | Linguagem principal do projeto                                            |
| **Django**          | Framework web para desenvolvimento rápido e seguro                       |
| **Django Ninja**    | Framework para criação de APIs rápidas e tipadas                         |
| **SQLite**          | Banco de dados padrão utilizado no desenvolvimento                       |
| **Pydantic/Ninja**  | Schemas para validação e serialização de dados                           |
| **Math (Python)**   | Utilizado para cálculos de progressão de faixas                          |

---
## 📡 Endpoints Principais

| Método | Endpoint                  | Descrição                                   |
|--------|---------------------------|---------------------------------------------|
| POST   | `/treino/`                | Criar novo aluno                            |
| GET    | `/treino/alunos/`         | Listar todos os alunos                      |
| GET    | `/treino/progresso_aluno/`| Consultar progresso de um aluno via email   |
| POST   | `/treino/aula_realizada/` | Registrar aulas realizadas para um aluno    |
| PUT    | `/treino/alunos/{id}`     | Atualizar dados de um aluno                 |

---

## DB
- SQLite3
  
---
# 🎨 Frontend - Sistema de Treino (Flet)

Interface gráfica desenvolvida em **Flet** para interação com a API do sistema de treino.  
Permite cadastrar alunos, listar registros, marcar aulas realizadas, consultar progresso e atualizar dados.

---

## 📌 Funcionalidades

- **Criar Aluno**: formulário para cadastro de novos alunos.
- **Listar Alunos**: tabela dinâmica exibindo todos os alunos cadastrados.
- **Cadastrar Aula**: marca aulas realizadas para um aluno específico.
- **Progresso do Aluno**: consulta o progresso do aluno (faixa atual, total de aulas e aulas necessárias para próxima faixa).
- **Atualizar Aluno**: edição de dados do aluno (nome, email, faixa, data de nascimento).

---

## ⚙️ Tecnologias Utilizadas

| Tecnologia        | Descrição                                                                 |
|-------------------|---------------------------------------------------------------------------|
| **Python 3.x**    | Linguagem principal                                                       |
| **Flet**          | Framework para criação de interfaces gráficas multiplataforma             |
| **Requests**      | Biblioteca para consumo da API REST                                       |
| **Django Ninja**  | API backend (projeto `treino`) que fornece os endpoints                   |

---

## Como executar o projeto

```bash
instalar o venv na pasta do projeto
--->python -m venv .venv
ativando venv
--->.\.venv\Scripts\Activate
baixando as dependencias
--->python -m pip install -r requirements.txt
--->python manage.py migrate
criar um superuser
--->python manage.py createsuperuser
executando o projeto
-->python manage.py runserver
```
---
# Autor

Guilherme Timm Moreira

