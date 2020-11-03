# Estilos e Padrões Arquiteturais - Parte 1

Neste módulo, será melhor explicado o que são Arquiteturas Monolíticas e Distribuídas, assim como uma breve introdução sobre Estilos Arquiteturais e Padrões Arquiteturais. Também será mostrado dois padrões arquiteturais, sendo eles o Stand-Alone e o N-Camadas.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 29/10/2020 | 1.0 | Criação do documento e adição das arquiteturas monolíticas e distribuídas, estilos arquiteturais, Stand Alone, N-Camadas | Micaella Gouveia |
| 03/11/2020 | 1.1 | Adição do padrão N-Camadas | Micaella Gouveia | 

## Arquiteturas Monolíticas
* Processamento centralizado
* Terminais 'Burros'
* Redes de comunicação mais lentas
* Sistema Timesharing
* Funcionalidades realizadas em um único processo em uma única instância de servidor e sua escalabilidade é conferida por replicação.
* Complicado extrair algo, uma funcionalidade legada, de forma escalável. Complicado incorporar algo, uma nova funcionalidade de forma escalável.

| Pontos Positivos | Pontos Negativos |
|-----------|--------------|
| Facilidade de gerência, seja em termos de segurança, controle de usuários e de aplicações |  Interface com o usuário limitada e usuário sem autonomia  |
|  | Arquiteturas de hardware, software e comunicação, normalmente, proprietárias, levando à dependência do fornecedor |
|  | Processamento centralizado, dificultando muito a questão de escalabilidade |
|  | Alto custo de manutenção e evolução |


## Arquiteturas Distribuídas
* Servidores de serviços compartilhados com boa capacidade de processamento.
* Estações de trabalho com bom poder de processamento, rodando aplicações locais, e sendo acessadas via interfaces gráficas.
* Redes com boa velocidade

| Pontos Positivos | Pontos Negativos |
|-----------|--------------|
| Usuário com autonomia | Sobrecarga da rede, pois as aplicações são executadas em estações, independentes, mas o acesso aos arquivos é feito em servidores|
| Interfaces com o usuário montada localmente e com recursos gráficos| Dificuldade de gerência, seja em termos de segurança, controle de usuários e aplicações|
| Processamento espalhado, permitindo o uso das aplicações nas estações| |
| Arquiteturas de software e comunicação podem ser proprietárias mas com recursos de integração entre plataformas||

## Estilos Arquiteturais
Uma arquitetura de software pode orientar-se por um estilo arquitetural. Trata-se de um conjunto de padrões, os quais procuram impor um determinado grau de uniformidade à arquitetura. São componentes e conectores específicos que funcionam como base
Expressa:
* Uma organização estrutural.
* Um conjunto pré-definido de substemas e suas responsabilidades
* Inclui regras e diretrizes para organizar o relacionamento entre os subsistemas


### Stand-Alone
Mais simples dos estilos arquiteturais. Basicamente, baseia-se em projetar uma solução autossuficiente, a qual não depende de terceiros. Normalmente, esses terceiros são servidores especializados em fornecer serviços e/ou conteúdos.
* Estilo indicado para projeto mais simples. Quando complexos, os projetos podem demandar soluções distribuídas, com comunicações entre clientes e servidores, P2P ou outro.

| Pontos Positivos | Pontos Negativos|
| - | - |
| Simplicidade| Limitação da capacidade do projeto de expandir|

### N-Camadas
Usado para modelar a interface dos subsistema, organiza o sistema em um conjunto de camadas, cada uma das quais fornece um conjunto de serviços. Esse padrão apoia o desenvolvimento incremental de subsistemas em diferentes camadas, e quando uma camada é alterada, normalmente, apenas a camada adjacente é afetada.

**CUIDADOS:**
* As camadas de níveis superiores dependem das camadas de níveis inferiores.
* Partes do sistema devem permitir serem trocadas
    * Trocar a camada de Comunicação
    * Trocar a camada de acesso
* Podem existir várias camadas em um mesmo nível de abstração, dependendo de camadas inferiores.

**DIRETRIZES:**
* Procure estruturar o sistema em camadas, sobrepondo as mesma em níveis de abstração diferentes.
* Lembre-se que os serviços da camada X, se dependentes de algo, que essa dependência esteja, preferencialmente restrita à camada X-1. (**Arquitetura Restrita**)
* Se houver necessidade de depender de mais de uma camada inferior (**Arquitetura Relaxada**)
* O inverso, ou seja, camadas inferiores dependerem de camadas superiores não é desejado!

| Pontos Positivos | Pontos Negativos|
| - | - |
| Reutilização de Camadas | Cascateamento de alterações para as camadas superiores, quando o comportamento de uma camada inferior sobre alteração /adaptações
| Dependências tendem a permanecer locais| 
| Flexibilidade para organizar multi-níveis de abstração| 
| Permite trabalhar com sistemas de dinâmicas complexas |

## Padrões Arquiteturais

### MVC (Model View Controller)
Esse padrão separa a apresentação e a interação de dados do sistema. Ele é estruturado em três camadas lógicas, as quais interagem entre si.

* **Model**: Detém a funcionalidade principal bem como os dados associados a cada entidade de domínio.
    * Encapsula estado da aplicação
    * *Notifica View de mudanças de estado*
* **View**: Lida com a exibição dos dados que são apresentados ao usuário.
    * Modelo renders
    * *Solicita atualização de models*
    * Envia eventos de usuário para controller.
* **Controller**: Gerencia a interaçao dos usuários e faz o intermédio das interações entre View e Model.
    * Mapeia ações de usuários para atualizar modelo.
    * Seleciona views

É usado quando existe várias maneiras de se visualizar e interagir com dados, também quando são desconhecidos os futuros requisitos de interação e apresentação de dados. É usado quando há necessidade de várias interfaces com o usuário, e/ou de várias visões de dados e/ou até de mudanças nos dados constantes.

### Estrutura Model
* Funcionalidade principal da aplicação
* Associar-se às controllers
* COnter os dados das entidades de domínio

### Estrutura View
* Criar e inicializar a controller associada
* Exibir informações ao usuário
* Implementar procedimento de atualização
* Recuperar dados da Model, sendo essa ação preferencialmente intermediada via Controller.

### Estrutura Controller
* Receber a entrada de dados e as requisições do usuário
* Transformar as requisições dos usuários em requisições à model
* Implementar o procedimento de atualização, se necessário.

| Vantagens | Desvantagens |
| - | - |
| Permite que os dados sejam alterados de forma independente de sua representação e vice-versa| Quando um modelo e as interfaces são simples, pode envolver o código adicinoal e maior complexidade de código desnecessária |
| Apoia a apresentação dos mesmos dados de maneiras diferentes, ou seja, múltiplas views de uma mesma model | Controllers e Views tendem a ser bem acopladas|
| Views sincronizadas| |
| Organização clara de abstrações ||

**Padrões de Projeto associados:**
1. GRASP (indireção e controller)
2. GoF Estrutural (Facade)
3. GoF Comportamental (Observer)

## Referências
-  ESTILOS E PADRÕES ARQUITETURAIS I - **Milene Serrano** - Disponível em: <https://aprender3.unb.br/pluginfile.php/26819/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais%20I%20-%20Profa.%20Milene.pdf>. Último acesso em 29/10/2020.
