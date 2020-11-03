# Estilos e Padrões Arquiteturais - Parte 2

Neste módulo, será melhor explicado alguns dos demais estilos arquiteturais, como o Cliente-Servidor, P2P, Objetos Distribuídos.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 03/11/2020 | 1.0 | Criação do documento e adição dos estilos arquiteturais Cliente-Servidor, P2P, Objetos Distribuídos| Micaella Gouveia |


## Estilo Cliente-Servidor
Estilo que separa clientes e servidores, sendo interligados entre si, geralmente utilizando uma rede de computadores. Cada instância de um cliente pode enviar requisições de dados para algum dos servidores conectados e esperar pela resposta. Por sua vez, algum dos servidores disponíveis podem aceitar essas requisições, processá-las, e retornar o resultado para o cliente.

* Entre o cliente e servidor existe um **Protocolo de Comunicação**.
* O cliente e servidor podem residir no mesmo sistema.
* A máquina servidor é um host que está executando um ou mais programas de servidor que partilham seus recursos com os clientes. 
* Um cliente não compartilha seus recursos, mas solicita um conteúdo ou serviço de um servidor.
* Os clientes iniciam sessoes do comunicação com os servidores que esperam as solicitações de entrada.

### Cliente
* Sempre inicia solicitações/requisições aos servidores.
* Espera e recebe respostas.
* Normalmente conecta-se a um pequeno número de servidores de uma só vez.
* Normalmente interage diretamente com os usuários finais por meio de interfaces, como interface gráfica.

### Servidor
* Sempre espera por uma solicitação/requisição de um dos clientes.
* Recebe as solicitações/requisições encaminhadas pelos clientes procurando respondê-las/atendê-las.
* Um servidor pode se comunicar com outros servidores, a fim de atender a uma solicitação/requisição do cliente.

| Pontos Positivos | Pontos Negativos |
|-----------|--------------|
| Na maioria dos casos, permite que as responsabilidades de um sistema possa ser distribuída entre vários computadores independentes, que estão conectados por meio de um rede. | Redes de tráfego  de bloqueio|
| Maior facilidade de manutenção (é possível substituir, reparar, atualizar ou realocar um servidor de seus clientes, minimizando os impactos dessa mudança)| Como o número de colicitações simultâneas de cliente para um determinado servidor pode ser razoável, o servidor pode ficar sobrecaregado|
| Todos os dados são armazenados nos servidores, que geralmente possuem controle de segurança muito superiores do que a maioria|  Elevado custo de comunicação|
| Servidores podem controlar mais adequadamente o acesso bem como os recursos, garantindo que apenas os clientes com as permissões apropriadas possam acessar e alterar dados | Não possui robustez como de uma rede P2P |
| Como o armazenamento de dados é centralizado, as atualizações desses dados são mais facilmente administrados.| Se um servidor crítico falhar, os pedidos dos clientes podem não ser cumpridos|
| Muitas tecnologias avançadas de cliente-servidor já estão disponíveis, muitas delas projetadas para garantir segurança, acessibilidade e usabilidade |

### Protocolos
Existem duas formas para que se estabeleça uma ligação cliente-servidor:

1. **Orientada a conexão (TCP - *Transmission Control Protocol*)**

O cliente estabelece uma conexão com o servidor e ambos trocam múltiplas mensagens de tamanhos variados, sendo a aplicação do cliente quem termina a sessão (Ex: email).

* Funcionamento mais complexos
* Mais controles, mais seguro em relação ao recebimento de dados
* Estabelece conexão antes de transmitir os dados (Transporte)
* Solicita retransmissão dos dados não recebidos ou corrompidos. 

2. **Não orientada à conexão (UDP - *User Datagram Protocol*)**

O cliente constói uma mensagem e a envia num pacote UDP para o servidor, o qual responde sem estabelecer uma conexão permanente com o cliente. Mais utilizado em aplicações de tempo real, por privilegiar velocidade e simplicidade (Ex: VolP)

* Funcionamento mais simples
* Mais rápidp por ter menos Controles
* Menos seguro em relação ao recebimento dos dados (Transporte)
* Não estabelece conexão

## Estilo P2P
É uma arquitetura de sistemas distribuídos caracterizada pela descentralização das funções na rede, onde cada nó realiza tanto funções de cliente quando de servidor.

**Responsabilidade do Peer como cliente**
* Enviar pedidos de serviço a outros peers
* Receber as respostas de pedidos de serviço feitos a outros peers.

**Responsabilidade do Peer como servidor**
* Receber pedidos de serviço de outros peers
* Processar os pedidos e xecutar o serviço requerido
* Enviar resposta com os resultados do serviço requerido
* Propagar os pedidos de serviço a outros peers

| Pontos Positivos | Pontos Negativos |
|-----------|--------------|
| Elimina o gargalo de fonte única, usando o P2P para distribuir dados e fazer o balancemaneto de pedidos na rede| Implementação bem mais complexa, demandando mais conhecimento da equipe de implantação e manuntenção
| ELimina o risco de um único ponto de falha | Overheads - Comunicações replicadas entre pares, ou seja, mesma busca sendo processada por muitos nó diferentes |
| A infraestrutura P2P permite acesso direto aos recursos compartilhados e isso confere capacidade de manutenção remota|

## Estilo Objetos Distribuídos
É uma arquitetura de sistemas distribuídos muito parecida com P2P, porém possui um Middleware, intermediando o processo de comunicação.

## Referências
-  ESTILOS E PADRÕES ARQUITETURAIS II - **Milene Serrano** - Disponível em: <https://aprender3.unb.br/pluginfile.php/26819/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais%20II%20-%20Profa.%20Milene.pdf>. Último acesso em 03/11/2020.