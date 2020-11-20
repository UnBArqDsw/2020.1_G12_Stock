# Reutilização de conexões Websockets

A reutilização de componentes de software existentes ou convenientemente disponíveis para reduzir tempo e custos de computação e recursos humanos é chamada de capacidade de reutilização de software.

A reutilização de software não envolve somente fatores técnicos, como a utilização de métodos, ferramentas ou métricas, mas também no nível de requisitos, projeto e outros.

## Histórico de Revisão

| Data       | Versão | Descrição                          | Autor        |
| ---------- | ------ | ---------------------------------- | ------------ |
| 20/11/2020 | 1.0    | Criação do documento               | Gabriel Davi |
| 20/11/2020 | 1.1    | Adição da reutilização do Frontend | Gabriel Davi |

## Web Sockets

É uma tecnologia de comunicação em tempo real entre o cliente e servidor, no qual o clinte recebe informações do servidor sem necessidade de enviar qualquer requisição para obte-lo.
Por isso, foi utilizado no frontend da aplicação uma função que assiste por conexões em socket para receber determinadas informaçẽos. No backend, uma função em específica fica responsável por distribuir tal informação para todas as aplicações conectadas via socket.

### Frozen Spots

São considerados aqueles pontos que permanecem fixos em todas as instanciações, representa uma arquitetura geral do sistema. Com o Socket, estamos utilizando alguns frozens spots, como:

- **Configuração**: Para toda configuração de um socket para NodeJS, tanto no backend quando no frontend é preciso seguir o padrão de criação de conexões e ligamento com essas conexões. No backend, criamos uma nova instância do servidor e passamos essa nova instância para bilbioteca de socket. No frontend, utilizamos a biblioteca de client para conectar a com o servidor socket.

_Conexão socket backend_

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/backend/configuracao-socket.png" class="codes-prints" />
</p>

_Conexão socket frontend_

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/configuracao-web-socket.png" class="codes-prints" />
</p>

**Assistir e mandar informações via socket**: A fim de mandar e receber informações via socket, precisamos seguir um padrão que faz parte do protocolo. Pra mandar uma informação, precisamos criar uma mensagem, que será o nome do "canal" que o frontend deverá esperar receber essas informações. No frontend, precisamos criar listeners que se conectam com tais "canais" e aguardam por qualquer informação.

_Enviando informações backend_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/backend/send-message.png" class="codes-prints" />
</p>

_Recebendo informações frontend_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/sendMessage-front.png" class="codes-prints" />
</p>

### Hot Spots

São considerados aqueles pontos que são projetados para serem genéricos, dando liberdade ao usuário de modelar como quiser. Representa partes específicas do sistema. No Socket, podemos configurar a estrutura como recebemos e enviamos nossas informação, canais de compartilhamento de informações e etc.

- **Parametros passados para conexão**: No momento em que um client e um frontend se conecta a um backend, podemos passar alguns parametros para conexão. Isso é útil quando queremos configurar nosssas conexões para terem comportamentos distintos de acordo com os parâmetros que ele receber.

_Frontend enviando parametros de conexão_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/conexão-socket-front.png" class="codes-prints" />
</p>

_Backend recebendo o parametro de conexão_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/parametros-socket.png" class="codes-prints" />
</p>

- **Infomações e "canais"**: Por mais que a forma como compartilhamos as informações via websocket seja padão, podemos definir dos canais de informações que podemos utilizar e as informações que enviamos.

_Backend enviando informações para o front por meio do canal update-product_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/canal-back.png" class="codes-prints" />
</p>

_Frontend assistindo por informações no canal update-product_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/canal-front.png" class="codes-prints" />
</p>

- **Função genérica para enviar informações para clients**: Em nosso projeto, foi criada uma função geral para envio de informações para clients. Ela espera uma message, que consiste no nome do canal que iremos compartilhar as informações, uma lista de clients conectados para receber a informação e por fim a informação a ser enviada.

_Função sendMessage_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/sendMessage.png" class="codes-prints" />
</p>

_uso da função send message_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/canal-back.png" class="codes-prints" />
</p>

**Função auxiliar para receber nova informação frontend**: Foi criado uma função auxiliar para receber novas informações no frontend. Ela facilita o uso universão, pois utliza do javascript para receber uma função como parâmetro que é modelada de acordo com o caso de uso.

_Exemplo da função subscribe_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/subcribe.png" class="codes-prints" />
</p>

_uso da função subscribe_

<p align="center">
  <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/architecture/frontend/subscribeUso.png" class="codes-prints" />
</p>

## Referências

- Websockets. Disponível em <https://developer.mozilla.org/pt-BR/docs/WebSockets#:~:text=WebSockets%20%C3%A9%20uma%20tecnologia%20avan%C3%A7ada,do%20usu%C3%A1rio%20e%20um%20servidor>. Último acesso em 20/11/2020.
