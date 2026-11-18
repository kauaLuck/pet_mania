#  PetMania - Sistema de Adoção e Gerenciamento de Pets

Aplicação Full Stack desenvolvida a partir de um projeto de desafio para o cadastro, visualização, edição e controle de disponibilidade de pets para adoção. Além da finalização completa das operações de CRUD na API RESTful em Java, este repositório inclui **correções de bugs e melhorias estruturais** no código original para garantir o funcionamento estável da aplicação e sua integração com o front-end.

---

##  Correções e Melhorias Implementadas

* **Correção de Bugs na API:** Resolução de falhas nas rotas e no tratamento das requisições para garantir respostas consistentes (`200 OK`).
* **Finalização do CRUD:** Implementação e validação completa das operações de criação, leitura, atualização e exclusão de registros.
* **Integração Back-end e Front-end:** Ajustes no consumo da API para exibir corretamente os cards, status de disponibilidade (*Disponível* / *Indisponível*) e imagens dos pets na interface.

---

##  Tecnologias Utilizadas

* **Back-end:** Java, Spring Boot, Maven
* **Front-end:** HTML5, CSS3, JavaScript
* **Testes de API:** Postman

---

##  Funcionalidades (CRUD)

* **Cadastrar Pet (`POST`):** Adiciona um novo animal com informações detalhadas (nome, espécie, raça, idade, sexo, porte, personalidade, foto e status de disponibilidade).
* **Listar Pets (`GET`):** Retorna todos os pets cadastrados no sistema.
* **Atualizar Pet (`PUT`):** Permite editar os dados ou alterar o status de adoção (*Disponível* / *Indisponível*).
* **Remover Pet (`DELETE`):** Exclui o registro de um animal do sistema.

---

##  Endpoints da API

A API roda localmente na porta `8080` através da rota base `/api/pets`.

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `GET` | `/api/pets` | Lista todos os pets cadastrados |
| `POST` | `/api/pets` | Cadastra um novo pet |
| `PUT` | `/api/pets/{id}` | Atualiza os dados de um pet existente |
| `DELETE` | `/api/pets/{id}` | Remove um pet pelo ID |

---

## 🧪 Testes da API com Postman

Após as correções no código, os endpoints foram validados utilizando o **Postman**:

### 1. Listagem de Pets (`GET /api/pets`)
Requisição retornando status `200 OK` com a lista de pets cadastrados em formato JSON:

<img width="1264" height="913" alt="Captura de tela 2026-11-11 165839" src="https://github.com/user-attachments/assets/b673cd84-e5d7-4a9a-8a5f-ed3b8615e485" />



### 2. Cadastro de Novo Pet (`POST /api/pets`)
Envio de payload JSON para criação de um novo registro, retornando status `200 OK` e o objeto criado com seu respectivo `id`:

<img width="1152" height="750" alt="Captura de tela 2026-11-11 170751" src="https://github.com/user-attachments/assets/ef83e8d3-c2b6-476c-bb7c-0609b8ec25b3" />


---

## 💻 Interface Web

Visualização da página principal exibindo os cards dos animais cadastrados e opções de gerenciamento funcionando após os ajustes:

<img width="1767" height="934" alt="Captura de tela 2026-11-11 170903" src="https://github.com/user-attachments/assets/287dce73-81ca-4699-9a81-6462af69535e" />



