  <h2>Arquitetura e desenho de software</h2>
  <h3>Sobre o projeto</h3>

  <p>Trata-se de um sistema para cadastro e consulta de estoque. Ele possui uma platarforma web para cadastro e listagem de produtos, bem como geração de planilhas com resumos e gráficos para mostrar sua evolução.Também, possui uma versão mobile somente para consulta rápida de produtos e para atualização mais ágil do estoque (Retirar um produto recém vendido, por exemplo) e por fim um servidor que irá cuidar de todo o fluxo do negócio. 
  </p>

  <h3>Membros da equipe</h3>

  <div class="members">
    <div class="member">
      <img src="./assets/img/members/GabrielDavi.jpg" alt="member name">
      <p>Gabriel Davi<p>
    </div>
    <div class="member">
      <img src="./assets/img/members/Gabriel.jpg" alt="member name">
      <p>Gabriel Alves<p>
    </div>
    <div class="member">
      <img src="./assets/img/members/Sofia.jpg" alt="member name">
      <p>Sofia Patrocínio<p>
    </div>
    </div>
    <div class="member line2">
    <div class="member">
      <img src="./assets/img/members/Micaella.jpg" alt="member name">
      <p>Micaella Gouveia<p>
    </div>
    <div class="member">
      <img src="./assets/img/members/Pedro.jpg"alt="member name">
      <p>Pedro Igor<p>
    </div>
   
  </div>
  <p align="center"><a href="https://fga.unb.br" target="_blank"><img width="230"src="https://4.bp.blogspot.com/-0aa6fAFnSnA/VzICtBQgciI/AAAAAAAARn4/SxVsQPFNeE0fxkCPVgMWbhd5qIEAYCMbwCLcB/s1600/unb-gama.png"></a></p>
  </p>
</div>

<style>
  .members {
    display: grid; 
    grid-template-columns: auto auto auto;
    margin-top: 20px;
  }
  .member img{
    position: relative;
    height: 200px;
    width: 200px;
    opacity: 1;
    border-style: solid;
    border-radius: 100px;
    border-width: 1px; 
    border-color: rgba(0,0,0,0.3);
    z-index: 3;
    transition: opacity 0.5s !important;
  }
  .member img:hover{
    opacity: 0.4;
    z-index: 1;
  }
  
 .member{
   margin: 20px;
   display: flex;
   justify-content: center;
  }
 
 .member p{
    position: absolute;
    transform: translate(0, 70px);
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
