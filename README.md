# LogiTrack - Sistema de Gerenciamento de Robôs Logísticos
Aplicação backend desenvolvida em Spring Boot com autenticação e autorização de usuários.

Inclui cadastro, login, gerenciamento de usuários e controle de acesso por roles (ADMIN e USER).

# Integrantes
- Erick Santos Santana RM: 559206
- Gabriel Borges Gonçalves Silva RM: 558861
- Rodrigo Vinzent Arinez Viscarra RM: 559192
- Tarik Omar Mazloum RM: 554933

## ⚙️ Tecnologias Utilizadas
- Java 17
- Spring Boot 3.4.4
- Spring Security
- H2 Database (memória)

## 🔑 Funcionalidades
- Registro e login de usuários
- Controle de permissões por roles
- Usuários padrão criados automaticamente

## ▶️ Como Executar
````
# Clonar repositório
git clone <repositorio>

# Entrar na pasta do projeto
Abrir <pasta-projeto>

# Rodar aplicação
Start
````
A API estará disponível em:
- http://localhost:8080

Banco de dados H2:
- http://localhost:8080/h2-console

## 🌐 Endpoints Principais
- POST /auth/login → Login com usuário/senha
- POST /auth/register → Cadastro de novo usuário
- GET /usuarios → Lista usuários 
- GET /usuarios/{id} → Busca usuário por ID
- PUT /usuarios/{id} → Atualiza usuário
- DELETE /usuarios/{id} → Remove usuário

## ⚒️ Alinhamento
Na versão mais recente do backend do LogiTrack, foram feitas melhorias importantes em relação à versão anterior:

- Adição de Spring Security + JWT para autenticação e autorização.
- Implementação de roles (ADMIN/USUARIO) para controle de acesso.
- Inclusão do CRUD de usuários com controle de perfil e permissões.
- Organização do código em pacotes: config, controller, dto, model, repository e service.
- Banco de dados: H2 para desenvolvimento e previsão de SQL em produção.
- Endpoints protegidos com anotações do Spring Security.