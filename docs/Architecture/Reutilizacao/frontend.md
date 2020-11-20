# Reutilização no Frontend

A reutilização de componentes de software existentes ou convenientemente disponíveis para reduzir tempo e custos de computação e recursos humanos é chamada de capacidade de reutilização de software. 

A reutilização de software não envolve somente fatores técnicos, como a utilização de métodos, ferramentas ou métricas, mas também no nível de requisitos, projeto e outros.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 19/11/2020 | 1.0 | Criação do documento e adição da reutilização do Frontend | Micaella Gouveia e Sofia Patrocínio |


A reutilização no Frontend se deu por meio de frameworks e bibliotecas, como ReactJS e Reactstrap.

## ReactJS

React é um framework de código-aberto para desenvolvimento de aplicações web baseado em Javascript, utilizando-se de uma arquitetura baseada em componentes.


https://unbarqdsw.github.io/2020.1_G12_Stock

### Frozen Spots
São considerados aqueles pontos que permanecem fixos em todas as instanciações, representa uma arquitetura geral do sistema. No React, estamos utilizando alguns frozens spots, como:

* **Hooks**: Permitem reutilizar lógica com estado sem mudar sua hierarquia de componentes.

*Exemplo de uso da hook useContext*

<p align="center">
<img src="assets/architecture/frontend/useContext.png" class="codes-prints" />
</p>

*Exemplo de uso da hook useState*

<p align="center">
<img src="assets/architecture/frontend/useState.png" class="codes-prints" />
</p>

*Exemplo de uso da hook useEffect*

<p align="center">
<img src="assets/architecture/frontend/useEffect.png" class="codes-prints" />
</p>

<br><br>

* **JSX**: Extensão de sintaxe para Javascript. É como uma linguagem de template, produzindo elementos do React.

*Exemplo de uso de JSX*

<p align="center">
<img src="assets/architecture/frontend/JSX.png" class="codes-prints" />
</p>

### Hot Spots
São considerados aqueles pontos que são projetados para serem genéricos, dando liberdade ao usuário de modelar como quiser. Representa partes específicas do sistema. No React, estamos utilizando alguns hot spots, como:

* **Componentes**: São como funções JavaScript. Eles aceitam entradas arbitrárias (chamadas “props”) e retornam elementos React que descrevem o que deve aparecer na tela.

*Exemplo de instância de um componente*

<p align="center">
<img src="assets/architecture/frontend/component.png" class="codes-prints" />
</p>



## Reactstrap
É uma biblioteca de UI baseada nos componentes do React, feita baseada no Bootstrap. Os atributos nesta biblioteca são usados   para passar o estado, aplicar classes modificadoras de maneira conveniente, habilitar funcionalidade avançada (como popperjs) ou incluir automaticamente elementos não baseados em conteúdo. 

*Exemplo de uso do Reactstrap*

<p align="center">
<img src="assets/architecture/frontend/reactstrap.png" class="codes-prints" />
</p>

## Referências
* Introdução aos Hooks. Disponível em <https://pt-br.reactjs.org/docs/hooks-intro.html#motivation>. Último acesso em 19/11/2020. 
* Introduzindo JSX. Disponível em <https://pt-br.reactjs.org/docs/introducing-jsx.html#:~:text=%C3%89%20chamada%20JSX%20e%20%C3%A9,produz%20%E2%80%9Celementos%E2%80%9D%20do%20React.>. Último acesso em 19/11/2020.