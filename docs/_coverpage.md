<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1,user-scalable=0"/>
    <img class="logo-image" src='./assets/Logo3_transparent.png'>
    <h1 class="tittle">O controle em sua mão</h1>
    <h3 class="legend">Com o Stock, você acompanha seu fluxo de estoque em tempo real.</h3>
<div class="content">
    <img class="bag" src="./assets/bag.svg">
    <img class="box" src="./assets/box.svg">
</div>

<style>
.cover:after {
    content: '';
    position: absolute;
    background-color: #F5F5F5;
}
.content {
    display: flex
}
.logo-image {
    margin-top: -10rem !important;
    width: 20rem;
    height: auto;
}

.tittle {
    margin-top: -6.0rem !important;
    font-family: Montserrat;
    color: #AC1C1C !important;
    font-size: 75 !important;
}

.legend {
    font-family: Montserrat;
    color: #1C1C1C !important;
    font-size: 30 !important;
    font-weight: 500;
}

.bag {
    @media screen and (max-width: 900px) {
        display: none
    }
    display: flex;
    position: absolute;
    left: -22.8rem;
    margin-top: -8rem;
}
.box {
    @media screen and (max-width: 900px) {
        display: none
    }
    display: flex;
    position: absolute;
    right: -22.8rem;
    margin-top: -8rem;
}



</style>
