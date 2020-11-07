  <h2>Arquitetura e desenho de software</h2>
  <h3>Sobre o projeto</h3>

  Trata-se de um sistema para [cadastro](Modeling/verbo?id=Cadastrar-Produto) e [consulta de estoque](Modeling/verbo?id=Consultar-Produto). Ele possui uma plataforma web para [cadastro](Modeling/verbo?id=Cadastrar-Produto) e listagem de produtos, bem como geração de planilhas com resumos e gráficos para mostrar sua evolução. Também, possui uma versão mobile somente para [consulta](Modeling/verbo?id=Consultar-Produto) rápida de produtos e para atualização mais ágil do [estoque](Modeling/objeto?id=Estoque) (Retirar um produto recém vendido, por exemplo) e por fim um servidor que irá cuidar de todo o [fluxo](Modeling/verbo?id=fluxo) do negócio. 
  

  <h3>Membros da equipe</h3>

  <div class="members">
    <div class="member">
      <p>Gabriel Davi</p>
      <img src="./assets/img/members/GabrielDavi.jpg" alt="member name">
    </div>
    <div class="member">
      <p>Sofia Patrocínio</p>
      <img src="./assets/img/members/Sofia.jpg" alt="member name">
    </div>
    </div>
    <div class="members">
    <div class="member">
      <p>Micaella Gouveia</p>
      <img src="./assets/img/members/Micaella.jpg" alt="member name">
    </div>
    <div class="member">
      <p>Pedro Igor</p>
      <img src="./assets/img/members/Pedro.jpg"alt="member name">
    </div>
    </div>
   
  </div>
  <p align="center"><a href="https://fga.unb.br" target="_blank"><img width="230"src="https://4.bp.blogspot.com/-0aa6fAFnSnA/VzICtBQgciI/AAAAAAAARn4/SxVsQPFNeE0fxkCPVgMWbhd5qIEAYCMbwCLcB/s1600/unb-gama.png"></a></p>
  </p>
</div>

<style>
  .members {
    display: flex; 
    flex-direction: row;
  }
  .member img{
    position: relative;
    width: 300px;
    opacity: 1;
    border-style: solid;
    border-radius: 200px;
    border-width: 1px; 
    border-color: rgba(0,0,0,0.3);
    z-index: 3;
    transition: opacity 0.5s !important;
  }
  .member img:hover{
    opacity: 0.4;
    z-index: 1;
  }
  .member p:hover  + img{
    opacity: 0.4;
    z-index: 1;
  }
  
 .member{
   display: flex;
   flex-direction: row;
   margin: 20px;
  }
 
 .member p{
    position: absolute;
    transform: translate(0, 4.8em);
    z-index: 2;
    color: #fff;
    font-weight: bold;
    font-family: Montserrat;
  }
 
  h2, p {
    font-family: Montserrat !important;
    font-weight: 500;
  }

  h3 {
    font-family: Montserrat !important;
    font-weight: bold;
  }
</style>
