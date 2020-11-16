# Estilos e Padrões Arquiteturais - Parte 3


Neste módulo, será melhor explicado alguns dos demais estilos arquiteturais, como o Filtros e Dutos e Repositório.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 16/11/2020 | 1.0 | Criação do documento | Micaella Gouveia |
| 16/11/2020 | 1.1 | Adição dos estilos filtros e dutos, repositório | Gabriel Davi |


## Estilo Filtros e Dutos

Oferece uma estrutura para sistemas que processam fluxos de dados, considerando a existÊncia de uma rede pela qual flui os dados de um extremidade (origem) à outra (destino).

* O fluxo de dados se dá através de pipes (dutos) e os dados sofrem transformações quando processados nos filters (filtros).
* Um duto provê uma forma unidirecional de fluxo de dados, uma vez que atua como um condutor para o fluxo de dados entre a fonte e o destino.
*  Divide uma grande tarefa de processamento em uma sequência de pequenos e independentes passos de processamento (Filters), os quais são conectados por canais (Pipes).

* **Filtro (Filter)**
1. Receber o dado da entrada
2. Processar o dado
3. Colocar o dado na saída

* ***Duto (Pipe)**
1. Transferir o dado
2. Realiza "buffer"
3. Sincronizar os filtros vizinhos

* **Outros Participantes**
1. Fontes de dados (Data source)
2. Coletor de dados (Dara sink)

| Vantagens | Desvantagens |
|-----------|--------------|
| O resultado é uma composição de filtros| Mudanças frequentes em um filtro impacta outros|
| Facilita o entendimento de Todo e Parte |Difícil uso em aplicações iterativas, pois coloca em ênfase o mado "batch"|
| Manutenabilidade mais flexível | Pode ter deadlock com o uso de buffers finitos|
| Facilita a reutilização, manutenção e extensão |
| Desempenho melhorado pelo processamento paralelo de filtros|

## Estilo Repositório
Subsistemas devem trocar dados. Isso pode ser feito de duas formas,
principais:
* Dados compartilhados são guardados em um banco de dados central ou
repositório, e podem ser acessados por todos os subsistemas, ou
* Cada subsistema mantém seu próprio banco de dados, e transmite dados
explicitamente para outros subsistemas.

Quando grandes quantidades de dados devem ser compartilhadas, é mais comum o uso do modelo de **repositório compartilhado**, sendo esse um eficiente mecanismo de compartilhamento de dados. Sendo que todos os dados em um sistema serão gerenciados em um único repositório central, acessível a todos os componentes do sistema. Os componentes não interagem entre si, apenas por meio deste repositório.

* Muito utilizado quabdo um sistema demanda grande volume de informação, que precisa ser geradoe armazenado por um longo tempo.
* Há também aplicabilidade ao estilo quando os sistemas são dirigidos a dados, nos quais a inclusão desses dados no repositório dispara uma ação

| Vantagens | Desvantagens |
|-----------|--------------|
| Os componentes podem ser independentes, então alterações feitas em um componente não costuma influenciar outro | O repositório é um ponto único de falha, problemas nele podem afetar o sistema todo |
| Todos os dados podem ser gerenciados de forma consistente, pois há centralização desses dados em um único repositório | Podem ocorrer ineficiências na organização de toda a comunicação por meio do repositório |
| | Distribuí-lo por meio de vários computadores pode ser complicado |


## Referências
-  ESTILOS E PADRÕES ARQUITETURAIS III - **Milene Serrano** - Disponível em: <https://aprender3.unb.br/pluginfile.php/26820/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais%20III%20-%20Profa.%20Milene.pdf>. Último acesso em 16/11/2020.