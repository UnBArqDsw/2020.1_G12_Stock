# Reutilização no Backend
**Para saber mais sobre Reutilização de Software acesse: [Reutilização de Software](Architecture/EstudoDirigido/reutilizacao.md)**

A reutilização de componentes de software existentes ou convenientemente disponíveis para reduzir tempo e custos de computação e recursos humanos é chamada de capacidade de reutilização de software. 

A reutilização de software não envolve somente fatores técnicos, como a utilização de métodos, ferramentas ou métricas, mas também no nível de requisitos, projeto e outros.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 19/11/2020 | 1.0 | Criação do documento | Micaella Gouveia |
| 19/11/2020 | 1.1 | Adição da reutilização do Backend | Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio|


A reutilização no Backend se deu por meio de frameworks e padrões de projetos, como NodeJS e padrão de projeto Decorator.

## NodeJS

NodeJS trata-se de um software open-source, cross-platform, e de um runtime de JavaScript que executa código de JavaScript a nível backend e frontend (dependendo apenas das bibliotecas e dos frameworks usados para esse mesmo fim). Ele possui hot spots e frozen spots, ambos estão sendo utilizados em nossa aplicação.

* **Hot Spots:**
    * Estrutura de pastas;
    * Tipagem (Typescript) - *não utilizado no projeto*.

* **Frozen Spots:**
    * Funções já embutidas (fileSystem, path, entre outros).


*Estrutura de pastas do Backend*

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/backend/pastas.png" class="codes-prints" />
</p>

## Decorator
O Decorator é um padrão de projeto que permite adicionar novos comportamentos a objetos através da adição de uma nova camada de um objeto externo que possui os comportamentos que deseja-se ser acrescentados. Ele traz um nível de reutilização de código pois o que é definido no Decorator pode ser aproveitado em outros níveis do sistema.

*Classe Decorator Base **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/Base.js))***

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/padroes/decorator/decoratorBase.png" class="codes-prints" />
</p>

*Collaborator herdando da Classe Decorator Base **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/CollaboratorBase.js))***

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/padroes/decorator/collaboratorBase.png" class="codes-prints" />
</p>


## Referências
* NodeJS. Disponível em <https://nodejs.org/en/about/>. Último acesso em 19/11/2020. 
