<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: <font color="red">??????????</font>

Nome:<font color="red">??????????</font>

<p><font color="red">Nota 5,4</font></p>

1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.
   2. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.
2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.
3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.
4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   1. (2.0 Pontos) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.
   2. (2.0) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:
   |CT|Valores de Entrada|Resultado esperado|
   |---|---|---|
   |||
   3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.


INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
5. Data da Entrega: 12/04/2022, as 22hs.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
7. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.

RESOLUÇÃO:

1.
   1. Processo de Testes de Software é um processo que tem como objetivo estruturar e dar forma às etapas, atividades, artefatos, papéis e responsabilidades do teste, permitindo assim a organização e controle de todo o ciclo por parte dos envolvidos.
   Projeto de Teste é o artefato responsável por gerenciar a fase de teste, identificando e descrevendo qual tipo de teste será aplicado e seus critérios de aprovação.
   Plano de Teste é o artefato responsável por identificar os elementos de software que serão testados, os recursos necessários para que sejam corretamente executados, abrangência, recomendações e descrições de estratégias de teste a serem aplicadas, e o cronograma de testes. <p><font color="red">Nota 0,5</font></p>

   2. Tanto o projeto quanto o plano de testes são artefatos gerados pela aplicação de um processo de teste em um produto de software. O plano de teste descreve os testes a serem executados numa visão de mais alto nível, enquanto o projeto descreve de forma mais detalhada os testes a serem executados. <p><font color="red">Nota 0,3</font></p>

2. Os testes ágeis permitem a identificação de defeitos em fases mais iniciais do processo de desenvolvimento, reduzindo o trabalho necessário para corrigi-los; fomenta um entendimento mais correto das necessidades dos usuários, evitando retrabalho; permite que os responsáveis por desenvolver e testar trabalhem cooperativamente, ao invés de numa relação de antagonismo. <p><font color="red">Nota 1,0</font></p>
3. Testes exploratórios são criados e executados simultaneamente, sem scripts ou de forma mais livre. Por basearem-se muito na intuição do testador, dependem bastante de seu conhecimento, habilidade e experiência. Seus elementos são exploração do produto, design de teste, execução de testes, heurística e revisão de resultados. <p><font color="red">Nota 1,0</font></p>
4.
   1. Cenários de Teste:
      |ID|Descrição| V/I |
	   |----|----|----|
	    |CE01|Número do banco contendo letras|I|
	    |CE02|Número do banco menor que três dígitos|I|
	    |CE03|Número do banco maior que três dígitos|I|
	    |CE04|Número do banco contendo três dígitos|V|
	    |CE05|Nome do banco contendo números|I|
	    |CE06|Nome do banco com menos de cinco letras|I|
	    |CE07|Nome do banco com mais de cem letras|I|
	    |CE08|Nome do banco contendo entre cinco e cem letras|V|
	    |CE09|Número da agência contendo letras|I|
	    |CE10|Número da agência menor que três dígitos|I|
	    |CE11|Número da agência maior que cinco dígitos|I|
	    |CE12|Número da agência contendo entre três e cinco dígitos|V|
	    |CE13|Nome da agência contendo números|I|
	    |CE14|Nome da agência com menos de cinco letras|I|
	    |CE15|Nome da agência com mais de cem letras|I|
	    |CE16|Nome da agência contendo entre cinco e cem letras|V|
	    |CE17|Nome da cidade contendo números|I|
	    |CE18|Nome da cidade com menos de cinco letras|I|
	    |CE19|Nome da cidade com mais de cem letras|I|
	    |CE20|Nome da cidade contendo entre cinco e cem letras|V|
	    |CE21|Número da conta contendo letras|I|
	    |CE22|Número da conta menor que seis dígitos|I|
	    |CE23|Número da conta maior que seis dígitos|I|
	    |CE24|Número da conta contendo seis dígitos|V|
	    |CE25|Tipo da conta diferente de 'Corrente' ou 'Poupança'|I|
	    |CE26|Tipo da conta igual a 'Corrente' ou 'Poupança'|V|
      <p><font color="red">Nota 1,5</font></p>
	 2. Casos de Teste:
        |CT|Valores de Entrada|Resultado esperado|
	     |----|----|----|
	      |CT01|12a|Inválido|
	      |CT02|53|Inválido|
	      |CT03|7515|Inválido|
	      |CT04|241|Válido|
	      |CT05|Banesp4|Inválido|
	      |CT06|Bco|Inválido|
	      |CT07|fasdlkjfdsalksdfjkfdsçaçlakjsdfjkldsasdriueiqwpkonmcçljvçalsdkurqhjnfdmca.lskcnvçlakuseiruknvkcçslaoisuerr|Inválido|
	      |CT08|Caixego|Válido|
	      |CT09|891G|Inválido|
	      |CT10|09|Inválido|
	      |CT11|2579541|Inválido|
	      |CT12|1121|Válido|
	      |CT13|Centra1|Inválido|
	      |CT14|Via|Inválido|
	      |CT15|fasdlkjfdsalksdfjkfdsçaçlakjsdfjkldsasdriueiqwpkonmcçljvçalsdkurqhjnfdmca.lskcnvçlakuseiruknvkcçslaoisuerr|Inválido|
	      |CT16|Perimetral|Válido|
	      |CT17|P4R15|Inválido|
	      |CT18|Una|Inválido|
	      |CT19|fasdlkjfdsalksdfjkfdsçaçlakjsdfjkldsasdriueiqwpkonmcçljvçalsdkurqhjnfdmca.lskcnvçlakuseiruknvkcçslaoisuerr|Inválido|
	      |CT20|Porangatu|Válido|
	      |CT21|124Y|Inválido|
	      |CT22|23578|Inválido|
	      |CT23|1354924|Inválido|
	      |CT24|415697|Válido|
	      |CT25|Conjunta|Inválido|
	      |CT26|Corrente|Válido|

        <p><font color="red">Nota 1,0</font></p>
