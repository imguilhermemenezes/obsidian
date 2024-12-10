
**Modelagem**: A modelagem é usada para criar representações abstratas de sistemas, auxiliando no entendimento, especificação, previsão e controle do comportamento do software.

**Elementos da UML**: Incluem classes, objetos, pacotes, e casos de uso, entre outros, como componentes básicos para construir modelos.

**Relacionamentos**: Descrevem conexões entre elementos da UML, como associação, generalização/especialização, dependência e agregação.

**Diagramas UML**: Ferramentas visuais para representar aspectos do sistema, como diagramas de classe, sequência, atividade e caso de uso.

**UML**: Notação que ajuda a definir requisitos, comportamento, estrutura lógica e dinâmica de processos. Não é uma linguagem de programação nem um processo de desenvolvimento.

**Visões na UML**:

- **Caso de Uso**: Interação entre sistema e agentes externos.
- **Projeto**: Estrutura e comportamento do software.
- **Implementação**: Gerenciamento de versões e subsistemas.

**Modelos de Casos de Uso (MCU)**:

- Criados por Ivar Jacobson, representam funcionalidades e interações do sistema com elementos externos.
- Componentes incluem casos de uso, atores e relacionamentos.
- Tipos de relacionamento: comunicação, inclusão, extensão e generalização.

**Casos de Uso e Atores**:

- Casos de uso são elipses descrevendo funcionalidades. Atores representam elementos externos que interagem com o sistema.
- Relacionamentos incluem comunicação, inclusão (cenários comuns), extensão (cenários opcionais) e generalização (herança de comportamento).

- **Conceito de Classes e Objetos**:
    
    - Representam entidades do sistema e suas interações, com estrutura (atributos) e comportamento (métodos).
    - Classes são representadas como caixas com até três compartimentos: nome, atributos e métodos.
- **Modelos de Classes (MC)**:
    
    - Evoluem durante o desenvolvimento iterativo do software.
    - Dividem-se em:
        - **Classes de Análise (MCA)**: Abstração inicial sem restrições tecnológicas.
        - **Classes de Especificação (MCE)**: Detalham as classes de análise, como analogia com partes estruturais de uma casa (encanamento, elétrica).
        - **Classes de Implementação (MCI)**: Implementadas em código, representando a programação final.
- **Diagramas de Classe**:
    
    - Utilizados para modelar o sistema, mostrando atributos, métodos e relacionamentos.
    - **Atributos**: Dados armazenados pelos objetos; variam entre instâncias.
    - **Métodos**: Ações executadas por objetos; compartilham comportamento entre instâncias.
- **Relacionamentos**:
    
    - **Associações**: Conexões entre objetos.
    - **Agregações**: Relação todo-parte, onde partes podem existir independentemente do todo.
    - **Composição**: Relação mais forte, onde partes dependem do todo para existir.
    - **Generalização/Especialização**: Representa herança entre classes (superclasse/subclasse).
- **Visibilidade**:
    
    - Níveis de acesso de atributos e métodos:
        - Pública (+): Acessível por qualquer objeto.
        - Privada (-): Restrita à classe.
        - Protegida (#): Acessível pela classe e suas subclasses.
        - De pacote (~): Acessível dentro do mesmo pacote.
- **Objetos**:
    
    - Instâncias das classes, definidas com atributos e métodos concretos.

### **Modelo de Sequência**

- **Finalidade**: Representar a sequência de eventos e interações entre objetos ou atores em um processo.
- **Base**: Diagrama de Caso de Uso e Diagrama de Classe, validando a relação entre os elementos.
- **Componentes Principais**:
    - **Atores**: Participantes externos ao sistema, representados com linhas de vida.
    - **Objetos**: Instâncias das classes, com linhas de vida que indicam sua existência durante o processo.
    - **Linha de Vida**: Mostra a duração da participação de objetos/atores; termina com um "X" quando o objeto é destruído.
    - **Foco de Controle**: Período de atividade de um objeto, indicado por uma linha grossa.
    - **Mensagens/Estímulos**:
        - Representam eventos que acionam métodos.
        - Podem ser entre atores, entre objetos ou entre ambos.
        - Incluem disparos de métodos, criação/destruição de objetos e mensagens de retorno.

### **Detalhes e Estereótipos**

- **Mensagens**:
    - Representadas por setas, que indicam comunicação e disparo de métodos.
    - Retornos são indicados com setas tracejadas.
- **Estereótipos**:
    - **Boundary**: Classes que conectam o sistema aos atores externos, geralmente relacionadas à interface.
    - **Control**: Intermediárias entre boundary e entidades, responsáveis por interpretar eventos e retransmiti-los.

### **Aplicações**

- Útil para modelar cenários detalhados em sistemas orientados a objetos.
- Ajuda a identificar métodos, eventos e responsabilidades.