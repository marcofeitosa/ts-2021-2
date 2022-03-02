
<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201905542
Nome: Marco Feitosa Araújo

<p><font color=green>Nota: 10,0.</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?
   O objetivo primário da atividade de teste de software é revelar a presença de defeitos no software sendo testado. <font color=green>Certo.</font>
    2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?
    Quando uma atividade de teste não revela a presença de defeitos, segue-se no ciclo de vida do teste para a etapa de revisão e auditoria e, posteriormente, para a de aceitação e baseline. <font color=green>Certo.</font>

2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.
O teste exaustivo é aquele que testa todas as possíveis combinações de entradas de dados, cenários e precondições em uma aplicação. Sua execução é impossível devido ao enorme gasto de tempo e recursos para o desenvolvimento de tantos cenários (um número exponencialmente maior quanto mais complexa for a aplicação). <font color=green>Certo.</font>
3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.
A técnica de Teste Funcional tem como limitações a dependência de uma boa especificação de requisitos para sua formulação (algo que muitas vezes não acontece), e a impossibilidade de garantir que partes essenciais ou críticas do software sejam executadas (sendo necessário um teste exaustivo para encontrar todos os defeitos).
A técnica de Teste Estrutural tem como limitações o possível grande número de caminhos de fluxo de controle (alguns dos quais podem acabar esquecidos no desenvolvimento dos testes), e a possibilidade de defeitos existirem mesmo em um fluxo de controle correto. <font color=green>Certo.</font>

4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.
O nível de Teste de Sistema trata do teste do sistema como um todo, com execução em condições similares àquelas em que o usuário o utilizará. Estes testes buscam verificar a conformidade do produto com requisitos funcionais e técnicos e padrões de qualidade, avaliando se os diversos componentes são todos compatíveis, se eles interagem corretamente entre si, se transferem os dados corretos no momento apropriado, etc. <font color=green>Certo.</font>

5. (**1.0 ponto**) escreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivlência.
O critério de Particionamento por Classes de Equivalência de testes funcionais tem como objetivo reduzir o número de casos de teste a serem desenvolvidos, sem com isso sacrificar a cobertura adequada do código sendo testado. <font color=green>Certo.</font>
6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.
Sim, existe uma hierarquia em relação aos critérios de teste estrutural. Segundo Copeland (2004), quanto maior o nível de cobertura (porcentagem dos requisitos testados x total de requisitos gerados), maior o rigor do critério do teste. Um teste **todos-nós** cobre todos os comandos do código, um teste **todos-arcos** cobre todas as decisões, e um teste **todos-caminhos** cobre todos os caminhos do código (decisões, condições, condições múltiplas, loops).
<font color=green>Certo.</font>
7. Considere a especificação, a seguir, de um hipotético programa que objtiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

**Observação**: A regra de existência do triângulo está errada no enunciado. Onde se lê "<", deve ser ">", e as condições devem ser atendidas simultaneamente, conforme consta na tabela de decisão abaixo.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.
![Tabela de decisão](https://github.com/marcofeitosa/ts-2021-2/blob/main/prova1_7.1.jpeg?raw=true)
<font color=green>Certo.</font>
7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:

Como três das nove hipóteses são matematicamente impossíveis, serão necessários apenas seis casos de teste:

|CT|Lado A|Lado B|Lado C|Resultado|
|---|---|---|---|---|
|CT01|6|4|10|Não é triângulo|
|CT02|3|3|3|Equilátero|
|CT03|4|4|5|Isósceles|
|CT04|3|4|4|Isósceles|
|CT05|3|4|3|Isósceles|
|CT06|2|3|4|Escaleno|

<font color=green>Certo.</font>

INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing
3. Forma de Entrega: Entregar este arquivo, editado com suas respostas, no formato .md, nominado da seguinte forma: ts2021-2_prova-p1_mat.md, onde mat deverá ser substituído pelo número da sua matrícula.
4. **Entrega diferente da especificada não será avaliada.**
5. Data da Entrega: 22/02/2022, as 23h59min.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.

RESOLUÇÃO:

1.
   1.

   2.

2.

3.


4.

5.

6.

7.
   1.
