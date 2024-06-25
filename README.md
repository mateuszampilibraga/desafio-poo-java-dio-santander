# Desafio de Modelagem e Diagramação de um Componente iPhone

## Descrição

Este repositório contém a solução para o desafio de modelagem e diagramação UML do componente iPhone, conforme descrito na trilha Java Básico da DIO. O objetivo do desafio era criar um diagrama UML que representasse as funcionalidades do iPhone como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

## Contexto

Com base no vídeo de lançamento do iPhone de 2007, foram identificadas e modeladas as seguintes funcionalidades:

- **Reprodutor Musical**
  - Métodos:
    - `tocar()`
    - `pausar()`
    - `selecionarMusica(String musica)`

- **Aparelho Telefônico**
  - Métodos:
    - `ligar(String numero)`
    - `atender()`
    - `iniciarCorreioVoz()`

- **Navegador na Internet**
  - Métodos:
    - `exibirPagina(String url)`
    - `adicionarNovaAba()`
    - `atualizarPagina()`

## Estrutura do Projeto

### Diagrama UML

O diagrama UML foi criado utilizando uma ferramenta de modelagem UML. Ele inclui:

![images/Modelagem_e_Diagramacao_iPhone.png](https://github.com/mateuszampilibraga/desafio-poo-java-dio-santander/blob/main/Modelagem%20e%20Diagrama%C3%A7%C3%A3o%20de%20um%20Componente%20iPhone.png)

- **Pacote `Main`**
  - Classe `iPhone` com atributos e métodos básicos.

- **Pacote `iPod`**
  - Interface `ReprodutorMusica` com os métodos `tocarMusica()`, `pausarMusica()`, e `selecionarMusica(String musica)`.
  - Interface `ReprodutorVideo` com métodos relacionados a reprodução de vídeo.

- **Pacote `Phone`**
  - Interface `AparelhoTelefonico` com os métodos `ligar(String numero)`, `atender()`, `iniciarCorreioVoz()`, e outros.
  - Outras interfaces relacionadas a funcionalidades de mensagens, galeria de imagens e calendário.

- **Pacote `Internet`**
  - Interface `NavegadorInternet` com os métodos `exibirPagina(String url)`, `adicionarNovaAba()`, e `atualizarPagina()`.
  - Outras interfaces relacionadas a serviços de e-mail, mapas e widgets.

### Implementação

As classes e interfaces foram implementadas em arquivos .java, seguindo a estrutura modelada no diagrama UML. As implementações estão organizadas nos seguintes pacotes:

- `main`: Contém a classe principal `iPhone`.
- `ipod`: Contém as interfaces relacionadas ao reprodutor musical e de vídeo.
- `phone`: Contém as interfaces relacionadas ao aparelho telefônico.
- `internet`: Contém as interfaces relacionadas ao navegador na internet e serviços adicionais.

## Como Executar

Para compilar e executar o projeto, siga os passos abaixo:

1. Clone o repositório:
    ```sh
    git clone https://github.com/mateuszampilibraga/desafio-poo-java-dio-santander.git
    ```

2. Navegue até o diretório do projeto:
    ```sh
    cd seu-repositorio
    ```

3. Compile os arquivos Java:
    ```sh
    javac -d bin src/**/*.java
    ```

4. Execute a classe principal:
    ```sh
    java -cp bin main.iPhone
    ```

## Conclusão

O diagrama UML foi criado para capturar todas as funcionalidades especificadas no desafio. A implementação das classes e interfaces segue rigorosamente o modelo proposto, garantindo que todas as funcionalidades do iPhone como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet estejam corretamente representadas e funcionais.
