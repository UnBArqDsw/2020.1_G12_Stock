# Estilos e Padrões Arquiteturais - Parte 4

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 02/11/2020 | 1.0 | Criação do documento e adição das arquiteturas Orientado a Eventos e Serviços| Pedro Igor |

## Estilo Arquitetural Orientado a Eventos
É um estilo arquitetural bastante utilizado em interfaces gráficas onde um evento na interface ocasiona funcionalidades sendo executadas.
Os eventos são gerados externamente. Pode ser um sinal com uma gama de valores ou uma série de comandos baseados em um menu. A ocorrência do evento está fora do controle do processo que o manipula. Esta é a diferença de um entrada simples.

O sistema precisa estar preparado para reagir de acordo com o evento que foi disparado.
Normalmente são baseados em dois modelos:

**Broadcast**: um evento é transmitido para todos os subsistemas e qualquer subsistema que for programado para manipular esse evento pode responder a ele.

**Orientado a interrupções**: Os eventos são recebidos por um tratador de interrupções que encaminha o evento para o componente responsável pelo processamento. São utilizados exclusivamente em sistemas de tempo real. Os próprios subsistemas decidem de quais eventos necessitam.

Todos os eventos podem ser transmitidos a todos os subsistemas porém não é recomendado por provocar overhead de processamento. Geralmente o tratador dos eventos mantém um registro dos subsistemas e eventos correspondentes. As classes responsáveis pelo tratamento de eventos são chamadas Listeners.

|Pontos Positivos|Pontos Negativos|
|----------------|----------------|
|Evolução é relativamente simples. | Subsistemas não sabem se ou quando os eventos serão manipulados.|
|Um novo subsistema para tratar classes específicas de eventos pode ser integrado por meio do registro de seus eventos no tratador de eventos.|É possível que subsistemas diferentes se registrem para os mesmos eventos, podendo causar conflitos quando os resultados de manipulação de eventos forem disponibilizados. |
|Qualquer subsistema pode ativar qualquer outro subsistema sem saber seu nome ou sua localização. |
|Os subsistemas podem ser implementados em máquinas distribuídas. |

## Orientado a Serviços

Surgiu da necessidade de acesso direto de repositório de informações por outros programas. Na época as informações eram convertidas em navegador web e não permitia que um programa consultasse uma série de catálogos. A solução por web services define os dados e como estes podem ser acessados. De forma geral, web services são recursos computacionais disponibilizados por outros programas de forma padronizada. É uma instância de uma noção mais geral de um serviço que independe da aplicação que usa o serviço.

### Etapas da utilização de um serviço

**1**: Um provedor implementa uma funcionalidade em um serviço e disponibiliza sua utilização. Para que um solicitante possa utilizar esse serviço, o provedor o hospeda(registra) de forma pública utilizando informações a respeito da funcionalidade daquele serviço.

**2**: Um solicitante utiliza esse serviço em sua aplicação respeitando os padrões de chamada e preparando o tratamento da resposta.

## Referências
-  ESTILOS E PADRÕES ARQUITETURAIS IV - **Milene Serrano** - Disponível em:
<https://aprender3.unb.br/pluginfile.php/26820/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais%20IV%20-%20Profa.%20Milene.pdf> Último acesso em: 02/11/2020