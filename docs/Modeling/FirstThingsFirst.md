# First Things First
O método First Things First é uma técnica de priorização de requisitos que analisa matematicamente o benefício, penalidade, custo e risco relativo de cada requisito para que seja calculada uma ordem de prioridade entre os requisitos. A técnica foi aplicada como um detalhamento do [MoSCoW](Modeling/MOSCOW.md), visto que esta classifica as histórias de [usuário](Modeling/objeto?id=usuário) em 4 status diferentes.

Sendo assim, foi feita uma filtragem dos requisitos avaliados como "prioritários" na técnica de [MoSCoW](Modeling/MOSCOW.md), isto é, requisitos avaliados como **Must**, **Should** ou **Could** sendo desconsiderados os requisitos avalidados como **Would**. Além disso, a técnica exige que requisitos totalmente dependentes de outros não participem dos cálculos para evitar situações onde um requisito B é avaliado como prioritário, porém depende de um requisito A, que não tem prioridade tão alta, seja implementado em conjunto ou previamente. É possível [consultar](Modeling/verbo?id=consultar-produto) a tabela dos [Requisitos não avaliados](Modeling/FirstThingsFirst.md?id=Requisitos-Não-Avaliados).

Como a técnica foi aplicada após a criação do [Backlog](Modeling/Backlog.md), foi utilizada a história do [usuário](Modeling/objeto?id=usuário) correspondente aos requisitos (requisitos funcional e os não funcionais atrelados) na avaliação para melhor entendimento no momento da discussão em grupo.

Foram utilizados os seguintes pesos:

|      Avaliação      | Peso |
|:-------------------:|:----:|
| Benefício Relativo  |   2  |
| Penalidade Relativa |   1  |
| Custo Relativo      |   1  |
| Risco Relativo      |  0.5 |

Cada item da avaliação foi avaliado em um número entre 1 e 5.

O valor é calculado pela fórmula:
```
Valor = Benefício * Peso do Benefício + Penalidade * Peso da Penalidade
```

A prioridade é calculada pela fórmula:
```
Prioridade = Valor% / (Custo% * Peso do Custo + Risco% * Peso do Risco)
```



## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 18/09/2020 | 1.0 | Priorização First Thins First. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 19/09/2020 | 1.1 | Adição da tabela, introdução e detalhamento da técnica e referências.              | Pedro Igor |
| 19/09/2020 | 1.2 | Adição da tabela de requisitos não avaliados.   | Pedro Igor | 
| 19/09/2020 | 1.3 | Linkagem dos léxicos e outras documentações.    | Pedro Igor | 



## First Things First
<div class="ritz grid-container" dir="ltr">
  <table class="waffle" cellspacing="0" cellpadding="0">
    <tbody>
      <tr style='height:20px;'>
        <td class="s0" dir="ltr">Requisitos</td>
        <td class="s0" dir="ltr">Desejo</td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 121px; left: -1px;">Benefício Relativo</div>
        </td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 141px; left: -1px;">Penalidade Relativa</div>
        </td>
        <td class="s1" dir="ltr">Valor Total</td>
        <td class="s1" dir="ltr">Valor %</td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 97px; left: -1px;">Custo Relativo</div>
        </td>
        <td class="s1" dir="ltr">Custo %</td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 97px; left: -1px;">Risco Relativo</div>
        </td>
        <td class="s1" dir="ltr">Risco %</td>
        <td class="s1" dir="ltr">Prioridade</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF28</a></td>
        <td class="s2" dir="ltr">Fazer o pedido de cadastro da minha empresa</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">1,923076923</td>
        <td class="s3">1,375661376</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF03</a></td>
        <td class="s2"><a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> itens no meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">3,846153846</td>
        <td class="s3">1,171171171</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF30</a></td>
        <td class="s2">Editar o <a href="#/Modeling/objeto?id=papéis-dos-colaboradores">nível de acesso de um colaborador</a></td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">11</td>
        <td class="s3">5,555555556</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">2,272727273</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">1,077212806</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF04</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01, RNF03, RNF05</a></td>
        <td class="s2"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> itens presentes no meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">1,019607843</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF25</a></td>
        <td class="s2"><a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> valor de cada produto</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">2,272727273</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,9792843691</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF06</a></td>
        <td class="s2" dir="ltr">No momento do cadastro de um item, adicionar <a href="#/Modeling/objeto?id=tag">tags</a> aos <a href="#/Modeling/objeto?id=produto">produtos</a> </td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">8</td>
        <td class="s3">4,04040404</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">2,272727273</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">3,846153846</td>
        <td class="s3">0,962962963</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF01</a></td>
        <td class="s2" dir="ltr">Realizar o login na aplicação</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">3,846153846</td>
        <td class="s3">0,8666666667</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF31</a></td>
        <td class="s2">Adicionar ou remover um colaborador da aplicação</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">14</td>
        <td class="s3">7,070707071</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,8425925926</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF02</a></td>
        <td class="s2" dir="ltr">Criar contas para meus funcionários com diferentes níveis de acessos</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,6797385621</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF15</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01</a></td>
        <td class="s2">Que a atualização dos dados seja feita assim que houver alguma modificação no <a href="#/Modeling/verbo?id=controle-de-estoque">controle do estoque</a>
        </td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">14</td>
        <td class="s3">7,070707071</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,5465465465</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF23</a></td>
        <td class="s2"><a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> mesmo <a href="#/Modeling/objeto?id=produto">produto</a> separados por diferentes lotes</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">11</td>
        <td class="s3">5,555555556</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,5209471767</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF08</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF02</a></td>
        <td class="s2" dir="ltr"><a href="#/Modeling/verbo?id=importação">Importar</a> uma <a href="#/Modeling/objeto?id=planilha">planilha</a> em excel com dados do meu <a href="#/Modeling/objeto?id=estoque">estoque</a> na aplicação</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,5205205205</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF17</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF03, RNF05</a></td>
        <td class="s2">Possuir uma versão mobile do aplicativo do <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">12</td>
        <td class="s3">6,060606061</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,4684684685</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF09</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF02</a></td>
        <td class="s2">Gerar <a href="#/Modeling/objeto?id=planilha">planilhas</a> de análise do <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">9</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,4684684685</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF14</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF02</a></td>
        <td class="s2" dir="ltr">Visualizar gráficos baseados no <a href="#/Modeling/verbo?id=fluxo">fluxo</a> de <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">11</td>
        <td class="s3">5,555555556</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,4294294294</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF10</a>, RNF01</td>
        <td class="s2"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> um <a href="#/Modeling/objeto?id=log">log</a> de remoção e adição de itens ao <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,4217356042</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF24</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF02</a></td>
        <td class="s2" dir="ltr">Gerar gráficos que marcam a quantidade de <a href="#/Modeling/objeto?id=produto">produtos</a>  por funcionários</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">8</td>
        <td class="s3">4,04040404</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,378870674</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s4"></td>
        <td class="s4"></td>
        <td class="s5">73</td>
        <td class="s5">52</td>
        <td class="s5">198</td>
        <td class="s5">100</td>
        <td class="s5">44</td>
        <td class="s5">100</td>
        <td class="s5">52</td>
        <td class="s5">100</td>
        <td class="s4"></td>
      </tr>
    </tbody>
  </table>
</div>

## Requisitos Não Avaliados
<div class="ritz grid-container" dir="ltr">
  <table class="waffle" cellspacing="0" cellpadding="0">
    <tbody>
      <tr style='height:20px;'>
        <td class="s0" dir="ltr">Desejo</td>
        <td class="s0" dir="ltr">Para que eu possa</td>
        <td class="s0" dir="ltr">Requisitos</td>
        <td class="s0" dir="ltr"><a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s0" dir="ltr">Motivo</td>
        <td class="s0" dir="ltr">Dependência</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Dar <a href="#/Modeling/verbo?id=feedback">feedbacks</a> ao suporte da aplicação</td>
        <td class="s1" dir="ltr">Relatar qualquer erro encontrado ou sugestões de novas funcionalidades</td>
        <td class="s1" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF27</a></td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s2">Avaliado como Would no <a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr"><a href="#/Modeling/verbo?id=baixa-em-produto">Remover</a> itens do <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td>
        <td class="s1" dir="ltr">Controlar vendas e <a href="#/Modeling/verbo?id=baixa-em-produto">remoções do estoque</a></td>
        <td class="s1" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF07</a></td>
        <td class="s1" dir="ltr">Must</td>
        <td class="s3" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> itens no meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF03</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1"><a href="#/Modeling/verbo?id=baixa-em-produto">Dar baixa</a> em um <a href="#/Modeling/objeto?id=produto">produto</a> pelo aplicativo mobile</td>
        <td class="s1">Vender ou <a href="#/Modeling/verbo?id=baixa-em-produto">remover produtos</a> mais facilmente</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF18</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF03, RNF05</a></td>
        <td class="s1" dir="ltr">Should</td>
        <td class="s3" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> itens no meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a>&quot; e &quot;Possuir uma
          versão mobile do aplicativo do <a href="#/Modeling/objeto?id=estoque">estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF03</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF17</a>,<a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF03, RNF05</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Definir a quantidade mínima de determinado <a href="#/Modeling/objeto?id=produto">produto</a></td>
        <td class="s1">Ser <a href="#/Modeling/verbo?id=alertar">notificado</a> quando um item estiver em <a href="#/Modeling/estado?id=estoque-baixo">baixa no estoque</a></td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF19</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> itens no meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF03</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Ter uma lista de <a href="#/Modeling/objeto?id=produto">produtos</a> solicitados por clientes que não estão disponíveis no <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s1">Adquirir esses <a href="#/Modeling/objeto?id=produto">produtos</a>  e disponibinizá-los no <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF22</a></td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no <a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr"><a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> um <a href="#/Modeling/objeto?id=produto">produto</a> adicionando seu valor de fábrica</td>
        <td class="s1" dir="ltr">Visualizar uma margem de lucro satisfatória</td>
        <td class="s1" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF32</a></td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no <a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr"><a href="#/Modeling/verbo?id=filtrar-produtos">Filtrar</a> a minha busca por uma categoria no <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td>
        <td class="s1">Acessar com facilidade os <a href="#/Modeling/objeto?id=produto">produtos</a>  relacionados a esta categoria</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF05</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> itens presentes no meu <a href="#/Modeling/objeto?id=estoque">estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF04</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01, RNF03, RNF05</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1"><a href="#/Modeling/verbo?id=filtrar-produtos">Filtrar</a> a busca de um <a href="#/Modeling/objeto?id=produto">produto</a> por nome e/ou preço</td>
        <td class="s1">Acessar com facilidade as informações sobre este produto</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF12</a></td>
        <td class="s1" dir="ltr">Should</td>
        <td class="s3" dir="ltr">Depende de &quot; <a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> itens presentes no meu <a href="#/Modeling/objeto?id=estoque">estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF04</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01, RNF03, RNF05</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Gostaria de, no momento da listagem, poder <a href="#/Modeling/verbo?id=filtrar-produtos">filtrar</a> os <a href="#/Modeling/objeto?id=produto">produtos</a>  pela data de adição</td>
        <td class="s1">Ter um melhor <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a> dos <a href="#/Modeling/objeto?id=produto">produtos</a>  que estão mais tempo parados no meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF13</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> itens presentes no meu <a href="#/Modeling/objeto?id=estoque">estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF04</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01, RNF03, RNF05</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> <a href="#/Modeling/objeto?id=produto">produtos</a>  que mais saem do meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s1">Saber quais <a href="#/Modeling/objeto?id=produto">produtos</a>  devo comprar em maior quantidade</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF26</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01</a></td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no <a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">No momento da listagem, poder <a href="#/Modeling/verbo?id=filtrar-produtos">filtrar</a> os <a href="#/Modeling/objeto?id=produto">produtos</a>  pela data de vencimento</td>
        <td class="s1">Ter um melhor <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a> dos <a href="#/Modeling/objeto?id=produto">produtos</a>  que estão para vencer</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF29</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> itens presentes no meu <a href="#/Modeling/objeto?id=estoque">estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF04</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01, RNF03, RNF05</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Ser alertado que um ou mais <a href="#/Modeling/objeto?id=produto">produtos</a>  estão com quantidades mínimas no <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s1">Reabastecer itens quando estiver em <a href="#/Modeling/estado?id=estoque-baixo">baixa no estoque</a></td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF20</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;Definir a quantidade mínima de determinado produto&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF19</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Ser alertado caso um <a href="#/Modeling/objeto?id=produto">produto</a> ultrapasse o seu <a href="#/Modeling/estado?id=prazo-de-validade">prazo de validade</a></td>
        <td class="s1">Organizar meu <a href="#/Modeling/objeto?id=estoque">estoque</a>, retirando este <a href="#/Modeling/objeto?id=produto">produto</a> vencido</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF21</a></td>
        <td class="s1" dir="ltr">Should</td>
        <td class="s5" dir="ltr">Depende de &quot;<a href="#/Modeling/verbo?id=cadastrar-produto"> Cadastrar</a> itens no meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a>&quot;.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF03</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Gerar gráficos que marcam o periodo por quantidade total de produto</td>
        <td class="s1" dir="ltr">Fazer uma análise melhor do crescimento geral do meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td>
        <td class="s1" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF24</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF02</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> um <a href="#/Modeling/objeto?id=log">log</a> de remoção e adição de itens ao <a href="#/Modeling/objeto?id=estoque">estoque</a>.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF10</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01</a></td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Gerar gráficos que marcam a quantidade de <a href="#/Modeling/objeto?id=produto">produtos</a>  por categoria</td>
        <td class="s1" dir="ltr">Saber a quantidade de <a href="#/Modeling/objeto?id=produto">produtos</a>  por categorias</td>
        <td class="s1" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF24</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF02</a></td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no <a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Visualizar a margem de lucro dos meus <a href="#/Modeling/objeto?id=produto">produtos</a>  </td>
        <td class="s1" dir="ltr">Precificar da melhor forma os <a href="#/Modeling/objeto?id=produto">produtos</a> </td>
        <td class="s1" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF33</a></td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no <a href="#/Modeling/MOSCOW"> MOSCOW</a></td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1"><a href="#/Modeling/verbo?id=filtrar-produtos">Filtrar</a> para consulta um <a href="#/Modeling/objeto?id=log">log</a> de remoção e adição de itens ao <a href="#/Modeling/objeto?id=estoque">estoque</a> de forma temporal</td>
        <td class="s1"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> o <a href="#/Modeling/verbo?id=fluxo">fluxo</a> de <a href="#/Modeling/objeto?id=estoque">estoque</a> em um período específico</td>
        <td class="s1"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF11</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01</a></td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> um <a href="#/Modeling/objeto?id=log">log</a> de remoção e adição de itens ao <a href="#/Modeling/objeto?id=estoque">estoque</a>.</td>
        <td class="s4" dir="ltr"><a href="#/Elicitation/RequisitosElicitados?id=requisitos-funcionais">RF10</a>, <a href="#/Elicitation/RequisitosElicitados?id=requisitos-não-funcionais">RNF01</a></td>
      </tr>
    </tbody>
  </table>
</div>

## Referências
 - First Things First: <https://www.processimpact.com/articles/prioritizing.pdf>. Último acesso em 19/09/2020