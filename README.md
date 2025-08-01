# Sistema de Agendamento de Tarefas

Este projeto faz parte do **Desafio de Projeto da DIO** na trilha .NET:  
**Construindo um Sistema de Agendamento de Tarefas com Entity Framework**

O objetivo é desenvolver uma **API RESTful** para gerenciamento de tarefas (To-Do List),  
permitindo criar, consultar, atualizar e excluir tarefas.

---

## 🚀 Tecnologias utilizadas

- **.NET 9 / ASP.NET Core Web API**
- **Entity Framework Core 9**
- **SQLite** (banco de dados local)
- **Swagger / Swashbuckle** (documentação e testes de endpoints)


---

## 📌 Endpoints disponíveis

| Verbo HTTP | Endpoint                       | Descrição                          |
|-----------|--------------------------------|------------------------------------|
| **GET**   | `/Tarefa/{id}`                 | Obter tarefa por ID                |
| **GET**   | `/Tarefa/ObterTodos`           | Listar todas as tarefas            |
| **GET**   | `/Tarefa/ObterPorTitulo`       | Filtrar tarefas pelo título        |
| **GET**   | `/Tarefa/ObterPorData`         | Filtrar tarefas pela data          |
| **GET**   | `/Tarefa/ObterPorStatus`       | Filtrar tarefas pelo status        |
| **POST**  | `/Tarefa`                      | Criar uma nova tarefa              |
| **PUT**   | `/Tarefa/{id}`                 | Atualizar uma tarefa existente     |
| **DELETE**| `/Tarefa/{id}`                 | Deletar uma tarefa                 |

### ✅ Visualização no Swagger

![Swagger Screenshot](Sistema%20de%20Agendamento%20de%20Tarefas.png)

---

## 📄 Exemplo de JSON para POST/PUT

```json
{
  "id": 0,
  "titulo": "Estudar Entity Framework",
  "descricao": "Praticar migrations e consultas LINQ",
  "data": "2025-08-01T10:00:00",
  "status": "Pendente"
}
