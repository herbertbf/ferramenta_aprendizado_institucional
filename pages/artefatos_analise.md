# Artefatos de Análise
[Exemplo de linkagem com ](/requisitos_funcionais.md#ancora1)
## Arquitetura de software escolhida

A arquitetura visão-modelo 4+1 foi desenvolvida por Philippe Cruchten com o objetivo de descrever o funcionamento de sistemas de software e é baseado no uso de múltiplas visões concorrentes. Ela foi utilizada neste projeto pois suas visões são usadas para mostrar o sistema sob várias perspectivas, como usuário final, desenvolvedores e gerentes de projetos.

As 4 visões de modelo são: visão lógica, visão de desenvolvimento, visão de processo e visão física. A visão de caso de uso é usada para ilustrar a arquitetura e representa a visão +1.

### Visão Lógica

Ilustra a funcionalidade que o sistema disponibiliza para o usuário final. Para esta finalidade foi utilizado os Diagramas de classes e o Digrama de Entidade Relacionamento Estendido (EER).

#### Diagrama de Classes de Domínio

É uma representação visual de classes conceituais ou objetos do mundo real em um domínio de interesse. Usando a notação UML, o modelo de domínio é ilustrado com um conjunto de diagramas de classes nos quais não são definidas operações.

#### Diagrama de Classes de Projeto
É utilizado para representar os objetos que o sistema irá manipular, suas operações ou serviços (métodos). Os métodos são responsáveis por manipular os atributos, efetuar ações que alterem o estado dos atributos, manipular as associações e relacionamentos entre as classes.

#### Diagrama Entidade Relacionamento Estendido (EER)

Modelos entidade-relacionamento estendidos são diagramas avançados de banco de dados bastante semelhantes aos diagramas ER regulares. Diagramas ER estendidos são modelos de alto nível que representam os requisitos e complexidades de bancos de dados complexos.

### Visão de desenvolvimento

Ilustra o sistema do ponto de vista do programador e se preocupa com o gerenciamento de projeto. Para isto foi utilizado o Diagrama de Componentes e Diagrama de Pacotes.

#### Diagrama de Componentes

Este diagrama permite a modelagem física de um sistema, através da visão dos seus componentes e relacionamentos entre os mesmos. Similar a um pacote, mas com um enfoque do empacotamento físico de código. Basicamente, um diagrama de componentes é composto por: componente, interface e relacionamentos. 

#### Diagrama de Pacotes

Diagramas de pacotes são diagrama estruturais comumente usados para simplificar os diagramas de classe complexos e organizar as classes em pacotes. Um pacote é uma coleção de elementos relacionados, incluindo diagramas, documentos, classes e pacotes de eventos.

### Visão de processo
Permite visualizar as partes dinâmicas do sistema, explicar os processos e como eles se comunicam, focando no comportamento do sistema. Para este processo normalmente é utilizado o Diagrama de Atividades, mas ele pode (e foi nesse projeto) ser substituído pelo Diagrama Business Process Model and Notation (BPMN) pois este também serve para modelar processos.

#### Diagrama Business Process Model and Notation (BPMN)

Um diagrama  BPMN é uma representação gráfica feita a partir de ícones que simbolizam o fluxo de processo. Ou seja, a partir dessa notação é possível fazer o mapeamento dos processos. Portanto, cada ícone representa uma etapa do processo de produção.

- Como é:

|![Coloque a descrição da sua imagem aqui, e o link coloque a seguir dentro dos parenteses](https://dtdsgp.com/wp-content/uploads/2020/05/news1.png)| 
|:--:| 
|*Legende aqui a sua imagem*|

- Como será: 
 
|![Coloque a descrição da sua imagem aqui, e o link coloque a seguir dentro dos parenteses](https://dtdsgp.com/wp-content/uploads/2020/05/news1.png)| 
|:--:| 
|*Legende aqui a sua imagem*|

### Visão física

Mostra como os executáveis e componentes são mapeados para plataformas e nós físicos, ou seja, a distribuição física de elementos do sistema.

#### Diagrama de Implantação

Este diagrama foca a questão da organização da arquitetura física sobe a qual o software irá ser implantado e executado em termos de hardware, ou seja, as máquinas (computadores pessoais, servidores etc.) que suportam o sistema, além de definir como estas máquinas serão conectadas e por meio de quais protocolos se comunicarão e transmitirão as informações.

### Visão de caso de uso

Descreve a arquitetura do sistema através do uso de Diagramas de casos de uso pois cada diagrama descreve sequências de interações entre os objetos e processos. 

#### Diagramas de caso de uso

Um modelo de caso de uso é um modelo que descreve como diferentes tipos de usuários interagem com o sistema para resolver um problema. Como tal, ele descreve as metas dos usuários, as interações entre os usuários e o sistema, bem como o comportamento necessário do sistema para satisfazer estas metas. 

#### Descrição de casos de uso

##### UC001 - Logar no sistema

- **Objetivo:**  Acessar o sistema.
- **Requisitos:** RF001.
- **Atores:** Técnico, Gestor B, Gestor A ou Gerente.
- **Gatilho:** Acessar o sítio eletrônico do sistema.
- **Pré-condição:** O ator deve estar cadastrado no sistema.
- **Pós-condição:**   
-  **Descrição tabular:** 
  
   - Fluxo principal:
  
|Sistema|Atores|
|:---:|:---:|
|-|1. Insere os dados de acesso.|
|-|2. Confirma os dados no sistema.|
|3. Verifica os dados.|-| 
|4. Concede acesso ao sistema.|-|      


- Fluxo Alternativo 1:
        
|Sistema|Atores|
|:---:|:---:|
|-|2. Envia dados inconsistentes. |
|3. Não concede acesso ao sistema.|-|
|4. Exibe mensagem de erro.|-|

 
   - Fluxo Alternativo 2:
        
|Sistema|Atores|
|:---:|:---:|
|4. Identifica que o usuário tentou fazer o login na página errada.|-|
|5. Redireciona para a página de login correta.|-|





