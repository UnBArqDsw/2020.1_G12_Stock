# Reutilização pelo Docker

A reutilização de componentes de software existentes ou convenientemente disponíveis para reduzir tempo e custos de computação e recursos humanos é chamada de capacidade de reutilização de software. 

A reutilização de software não envolve somente fatores técnicos, como a utilização de métodos, ferramentas ou métricas, mas também no nível de requisitos, projeto e outros.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 19/11/2020 | 1.0 | Criação do documento | Micaella Gouveia |
| 19/11/2020 | 1.1 | Adição da reutilização do Docker | Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio|

## Docker
Uma das formas de reutilização no projeto foi por meio da utilização do Docker.
O Docker simplifica e acelera o fluxo de trabalho, dando aos desenvolvedores a liberdade de inovar com sua escolha de ferramentas, pilhas de aplicativos e ambientes de implantação para cada projeto. Ele possui muitos hot spots, e alguns frozen spots, ambos estão sendo utilizados em nossa aplicação. Utilizamos o Docker Compose para orquestrar os containers do Docker.

* **Frozen Spots**:
    * Formatação do arquivo;
    * Nome dos arquivos

* **Hot Spots**:
    * Imagem para construir o container;
    * Dependências;
    * Comandos que o container executa ao iniciar;
    * Network;
    * Variáveis de ambiente


*Exemplo do dockerfile*

<p align="center">
<img src="assets/architecture/docker/dockerfile.png" class="codes-prints" />
</p>

*Exemplo do docker-compose*

<p align="center">
<img src="assets/architecture/docker/dockercompose.png" class="codes-prints" />
</p>


### Docker Frontend
Para o Frontend, foi configurado um Docker utilizando as tecnologias do React, utilizando a mesma base do NodeJs. Ele também fica responsável em padronizar as versões das bibliotecas utilizadas, impedindo que haja conflitos de desenvolvimento entre os membros do time. 


### Docker Backend
Para o Backend, foi configurado um Docker utilizando as tecnologias do NodeJs. Ele também fica responsável em padronizar as versões das bibliotecas utilizadas, impedindo que haja conflitos de desenvolvimento entre os membros do time. 

### Docker Conjunto
Para rodar a aplicação, é necessário subir tanto o Docker do Front como o do Back. Para facilitar o desenvolvimento, foi criado um Docker conjunto, que fica responsável tanto pelo Front como Back. Ele ajuda bastante pela sua praticidade, pois agora com um comando conseguimos subir toda a aplicação, além de poder visualizar eventuais defeitos em um só lugar/terminal.

*Docker-compose do Docker Conjunto*

<p align="center">
<img src="assets/architecture/docker/dockerConjunto.png" class="codes-prints" />
</p>

## Referências
* Why Docker. Disponível em <https://www.docker.com/resources/what-container>. Último acesso em 19/10/2020.
* Docker Compose. Disponível em <https://docs.docker.com/compose/>. Último acesso em 19/11/2020.
