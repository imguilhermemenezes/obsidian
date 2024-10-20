# **Documentação do Projeto: To-Do List com Streaks**

## **1. Descrição Geral**
Este aplicativo será um gerenciador de tarefas (To-Do List) com um sistema de **streaks (ofensiva)**, no qual os usuários ganham um dia a mais de ofensiva ao completar tarefas diárias e perdem a sequência se não completarem. O aplicativo também enviará **notificações** diárias para lembrar os usuários de suas tarefas e da necessidade de manter a ofensiva.

## **2. Funcionalidades Principais**

### 2.1 **Gerenciamento de Tarefas**
- **Criar tarefa**: O usuário pode criar uma nova tarefa com título, descrição e prazo.
- **Editar tarefa**: O usuário pode editar o título, descrição e prazo de uma tarefa.
- **Excluir tarefa**: O usuário pode remover uma tarefa.
- **Marcar como concluída**: O usuário marca a tarefa como feita, o que contribui para o progresso da ofensiva.
- **Categorias**: O usuário pode categorizar suas tarefas (ex: Pessoal, Trabalho, Estudo).
- **Prioridade**: Adicionar nível de prioridade (Baixa, Média, Alta) para cada tarefa.

### 2.2 **Sistema de Streaks (Ofensiva)**
- **Contador de Streak**: Cada vez que o usuário marca todas as tarefas diárias como concluídas, ele mantém ou aumenta seu streak.
- **Perda de Streak**: Se o usuário não completar as tarefas diárias, o streak é zerado.
- **Histórico de Streaks**: O usuário pode visualizar o número de dias consecutivos em que completou todas as suas tarefas.

### 2.3 **Notificações e Lembretes**
- **Notificações diárias**: Notificações push serão enviadas ao usuário durante o dia para lembrar de completar suas tarefas.
- **Notificações personalizadas**: O usuário pode definir horários específicos para ser notificado sobre cada tarefa.
- **Notificação de perda de streak**: Caso o usuário não complete suas tarefas diárias, será enviada uma notificação alertando sobre a perda de streak.

### 2.4 **Autenticação e Perfis de Usuário**
- **Cadastro de usuário**: O usuário pode se registrar no app usando e-mail/senha, Google ou Facebook.
- **Login**: Login seguro com autenticação por e-mail/senha ou via redes sociais.
- **Perfil de usuário**: Cada usuário tem um perfil com seu nome, e-mail, avatar e histórico de streaks.
- **Sincronização em nuvem**: Sincronização das tarefas e streaks na nuvem para garantir que o usuário possa acessar de diferentes dispositivos.

### 2.5 **Painel de Estatísticas**
- **Relatório de tarefas concluídas**: Gráficos com a quantidade de tarefas concluídas em uma semana, mês, ou período personalizado.
- **Histórico de streaks**: O usuário pode ver um histórico detalhado de suas ofensivas.
- **Metas de desempenho**: Possibilidade de definir metas semanais/mensais de tarefas concluídas e monitorar o progresso.

## **3. Requisitos Funcionais**

### 3.1 **Frontend (App Mobile)**
- **Tecnologia**: React Native
- **Funcionalidades**:
  - Interface de usuário responsiva com opções de criar, editar e excluir tarefas.
  - Exibição de streaks e notificação ao usuário sobre progresso.
  - Painel de estatísticas com gráficos.
  - Autenticação via redes sociais e e-mail/senha.
  - Sistema de notificações integradas.

### 3.2 **Backend**
- **Tecnologia**: Node.js com Express.js
- **Banco de dados**: MongoDB (com MongoDB Atlas para armazenamento na nuvem)
- **Funcionalidades**:
  - CRUD (Create, Read, Update, Delete) para tarefas.
  - Manutenção de streaks do usuário (incremento e reinício de streaks).
  - Armazenamento de perfis de usuário e histórico de tarefas.
  - Integração com Firebase Cloud Messaging para envio de notificações push.

### 3.3 **Sistema de Notificações**
- **Tecnologia**: Firebase Cloud Messaging (FCM)
- **Funcionalidades**:
  - Notificações push diárias para lembrar o usuário de suas tarefas.
  - Notificações personalizadas com base no horário configurado pelo usuário.
  - Notificações de perda de streak.

### 3.4 **Autenticação e Segurança**
- **Autenticação via e-mail/senha**: Implementar com Firebase Authentication ou Passport.js.
- **Login via redes sociais**: Integração com Google, Facebook e Apple ID.
- **Segurança de Dados**: Utilizar HTTPS para todas as requisições e JWT (JSON Web Tokens) para autenticação.

### 3.5 **Persistência e Sincronização**
- **Banco de Dados**: MongoDB (armazenamento na nuvem)
- **Sincronização**: Todos os dados do usuário, incluindo tarefas e streaks, devem ser sincronizados entre diferentes dispositivos.

## **4. Arquitetura do Sistema**

### 4.1 **Arquitetura Frontend**
- **React Native** para desenvolvimento cross-platform (iOS/Android).
- **Redux** ou **Context API** para gerenciamento de estado.
- **Axios** para fazer requisições HTTP ao backend.

### 4.2 **Arquitetura Backend**
- **Node.js** com **Express.js** para construir APIs RESTful.
- **MongoDB** para armazenar dados de tarefas, usuários e histórico de streaks.
- **JWT** (JSON Web Token) para autenticação e autorização.
- **Firebase Cloud Messaging** para gerenciamento e envio de notificações push.

## **5. Requisitos Não Funcionais**

### 5.1 **Desempenho**
- O aplicativo deve ser rápido, com tempos de resposta para carregar e salvar tarefas inferior a 1 segundo.
- Suportar até 10.000 usuários simultâneos.

### 5.2 **Segurança**
- As credenciais dos usuários devem ser armazenadas de maneira segura com criptografia (por exemplo, com bcrypt).
- Toda a comunicação deve ser feita através de HTTPS.

### 5.3 **Escalabilidade**
- O sistema deve ser escalável para suportar um aumento no número de usuários sem degradação de desempenho.
- Uso de MongoDB Atlas para banco de dados escalável.

### 5.4 **Manutenibilidade**
- Código modular e bem documentado para facilitar futuras atualizações e manutenção.

## **6. Cronograma de Desenvolvimento**

| Fase                        | Tarefas                                                                  | Duração (dias) |
| --------------------------- | ------------------------------------------------------------------------ | -------------- |
| Planejamento                | Definição de requisitos e design do sistema                              | 5              |
| Desenvolvimento do Backend  | Criar API, sistema de autenticação e banco de dados                      | 15             |
| Desenvolvimento do Frontend | Interface de usuário, criação de tarefas, integração com API             | 20             |
| Sistema de Notificações     | Implementação de notificações com Firebase Cloud Messaging               | 5              |
| Testes                      | Testes unitários e de integração                                         | 10             |
| Lançamento Beta             | Lançamento para testes beta                                              | 7              |
| Ajustes Finais e Lançamento | Revisão de feedback e ajustes finais, lançamento na Play Store/App Store | 10             |

## **7. Tecnologias Utilizadas**

- **Frontend**: React Native, Redux/Context API, Axios
- **Backend**: Node.js, Express.js, MongoDB, JWT
- **Notificações**: Firebase Cloud Messaging (FCM)
- **Autenticação**: Firebase Authentication ou Passport.js com JWT
- **Banco de Dados**: MongoDB Atlas (nuvem)