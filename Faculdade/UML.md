
### **Modelagem**
- Representa sistemas abstratamente para compreender, especificar, prever e controlar o comportamento do software.

### **Elementos da UML**
- Componentes básicos: classes, objetos, pacotes, casos de uso.

### **Relacionamentos**
- Tipos:
  - **Associação**: Conexão entre elementos.
  - **Generalização/Especialização**: Herança entre elementos.
  - **Dependência e Agregação**: Relacionamento todo-parte.

### **Diagramas UML**
- Representa aspectos do sistema:
  - Diagrama de classes.
  - Diagrama de sequência.
  - Diagrama de atividade.
  - Diagrama de caso de uso.

### **UML**
- Define requisitos, comportamento, estrutura lógica e processos dinâmicos.
- **Não é** linguagem de programação nem processo de desenvolvimento.

### **Visões na UML**
- **Caso de Uso**: Interação entre sistema e agentes externos.
- **Projeto**: Estrutura e comportamento do software.
- **Implementação**: Gerenciamento de versões e subsistemas.

---

### **Modelos de Casos de Uso (MCU)**
- Criados por Ivar Jacobson, representam funcionalidades e interações externas ao sistema.
- **Componentes**:
  - Casos de uso, atores e relacionamentos.
- **Relacionamentos**:
  - **Comunicação**.
  - **Inclusão** (cenários comuns).
  - **Extensão** (cenários opcionais).
  - **Generalização** (herança de comportamento).

### **Casos de Uso e Atores**
- **Casos de Uso**: Elipses que descrevem funcionalidades.
- **Atores**: Elementos externos que interagem com o sistema.

---

### **Conceito de Classes e Objetos**
- Representam entidades do sistema com:
  - **Atributos** (dados).
  - **Métodos** (funções/comportamentos).
- Classes são caixas com três compartimentos: nome, atributos e métodos.

### **Modelos de Classes (MC)**
- **Fases**:
  - **Classes de Análise (MCA)**: Sem restrições tecnológicas.
  - **Classes de Especificação (MCE)**: Detalhamento técnico.
  - **Classes de Implementação (MCI)**: Representam o código.

### **Diagramas de Classe**
- Modelam o sistema mostrando:
  - **Atributos**: Dados armazenados pelos objetos.
  - **Métodos**: Ações executadas pelos objetos.
- **Relacionamentos**:
  - **Associação**: Conexão entre objetos.
  - **Agregação**: Relação todo-parte independente.
  - **Composição**: Relação todo-parte dependente.
  - **Generalização/Especialização**: Herança entre classes.
- **Visibilidade**:
  - Pública (+), Privada (-), Protegida (#), De pacote (~).
- **Objetos**: Instâncias das classes.

---

### **Modelo de Sequência**
- **Finalidade**: Representar eventos e interações entre objetos ou atores.
- **Base**: Diagrama de Caso de Uso e Diagrama de Classe.
- **Componentes**:
  - **Atores**: Representados com linhas de vida.
  - **Objetos**: Instâncias de classes com linhas de vida.
  - **Linha de Vida**: Mostra existência durante o processo.
  - **Foco de Controle**: Indica atividade do objeto.
  - **Mensagens/Estímulos**: Representam eventos que acionam métodos, criação/destruição de objetos e mensagens de retorno.

### **Detalhes e Estereótipos**
- **Mensagens**:
  - Representadas por setas (disparo de métodos).
  - Retornos: Setas tracejadas.
- **Estereótipos**:
  - **Boundary**: Conectam o sistema aos atores externos.
  - **Control**: Intermediárias entre boundary e entidades.

---

### **Histórias de Usuário**
- **Definição**: Representação informal e clara de requisitos do usuário.
- **Estrutura**:
  - `COMO [tipo de usuário], EU QUERO [ação], PARA [resultado esperado].`
- **Vantagens**:
  - Simplicidade e agilidade.
  - Melhor visualização do valor agregado.
  - Flexibilidade no desenvolvimento.
- **Critérios de Aceitação**:
  - Validam se os requisitos foram atendidos.
  - Checklist para verificação.

### **User Stories e BDD**
- **BDD (Behavior Driven Development)** complementa histórias de usuário.
  - Estrutura: DADO QUE [cenário], QUANDO [ação], ENTÃO [resultado].

---

### **Tipos de Notação e Formatos de Casos de Uso**
- **Tipos**:
  - Diagramático: Diagrama de Caso de Uso (UML).
  - Textual: Documentação de Casos de Uso.
- **Formatos**:
  - Resumido: Breve cenário de sucesso.
  - Completo: Inclui interessados, condições e fluxos principais/alternativos.
  - **Abstrato**: Análise sem detalhes técnicos.
  - **Concreto**: Inclui detalhes de implementação.

### **Exemplo de Caso de Uso: Emprestar Livro**
- **Ator Principal**: Atendente.
- **Interessados**: Atendente, leitor, bibliotecário.
- **Fluxo Principal**:
  - Leitor solicita empréstimo → Sistema valida → Livros desmagnetizados → Leitor sai com os livros.
- **Fluxos Alternativos**:
  - Leitor desiste ou possui pendências.
  - Livro reservado ou restrito.

---

### **Diferenças: User Stories vs. MCUs**
- **User Stories**: Linguagem simples, focada no resultado desejado.
- **MCUs**: Documentação detalhada do comportamento do sistema.

---

### **Exercícios para Prática**
- Modelar casos de uso para:
  - Sistema de controle de encomendas.
  - Controle de solicitações e compras de materiais para construção.

