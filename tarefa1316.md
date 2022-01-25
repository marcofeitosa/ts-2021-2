## Tarefa 004 - 19/01/2022 - Análise do Valor Limte - Definição de casos de testes.

**DEFINIÇÃO**:
1. Considerando o conjunto de classes de equivalência que você definiu em atendimento à **Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência**.
2. Considerando as explicações a respeito do critério de teste funcional **Análise do Valor Limite** disponíveis em:
   1. [Análise do Valor Limite 1](https://viniciuspessoni.com/2020/03/15/analise-do-valor-limite/).
   2. [Análise do Valor Limite 2](https://www.youtube.com/watch?v=EQU5ODvmwzs).
   3. [Análise do Valor Limite 3](https://www.youtube.com/watch?v=jX7uyaTAn-k).
3. Pede-se a definição do conjunto de casos de testes necessários para o teste do mesmo cenário descrito na tarefa 003. Estes casos de teste deverão ser criadas a partir das diretrizes definidas pelo critério funcional "Análise do Valor Limte".
4. O Conjunto de casos de testes derivado deve seguir o seguinte padrão:

|CT|Valor de Entrada|Resultado Esperado|Classe Equivalência|
|--|--|--|--|
|CT01|-2|Valor Inválido|CE1|

Onde:
**CT** = Caso de Teste, seguido de um valor sequencial;
**Valor de entrada** é o valor informado para a variável;
**Resultado esperado** é o resultado que se espera da execução da função;
**Classe de Equivalência** é a identificação de qual classe de equivalência está sendo exercitada pelo caso de teste.

INSTRUÇÕES:
1. Tipo: Esta tarefa é individual;
2. Como responder: Pode-se editar este arquivo, complementando as tabelas de definições de classes de equivalência e dos casos de teste.
3. Local de Entrega: A entrega deverá seu repositório pessoal, utilizado para a manutenção dos artefatos de trabalho da disciplina (ts-2021-2);
4. Data da Entrega: Esta tarefa deve estar disponível para avaliação até o dia 24/01/2022 às 23h59min.
5. Esta tarefa valerá nota e presença para aula assíncrona do dia 18/01/2022.
6. Critério de Aceitação: tarefa entregue conforme especificado e na data definida.
7. Caso necessite de suporte, pode encaminhar mensagem para o professor.

RESOLUÇÃO:
|id|descrição|V/I|
|--|--|--|
|CE01|nota1 < 0|I|
|CE02|nota1 > 10|I|
|CE03|0 < nota1 < 10|V|
|CE04|nota1 tem mais que duas casas decimais|I|
|CE05|nota1 tem duas ou menos casas decimais|V|
|CE06|nota2 < 0|I|
|CE07|nota2 > 10|I|
|CE08|0 < nota2 < 10|V|
|CE09|nota2 tem mais que duas casas decimais|I|
|CE10|nota2 tem exatamente duas casas decimais|V|
|CE11|cargaHoraria < 1|I|
|CE12|cargaHoraria >= 1|V|
|CE13|cargaHoraria tem casas decimais|I|
|CE14|cargaHoraria é número inteiro|V|
|CE15|faltas < 0|I|
|CE16|faltas > cargaHoraria|I|
|CE17|0 <= faltas <= cargaHoraria|V|
|CE18|faltas tem casas decimais|I|
|CE19|faltas é número inteiro|V|
|CE20|faltas > cargaHoraria * 0.25|V|
|CE21|faltas < cargaHoraria * 0.25|V|
|CE22|media < 3.0|V|
|CE23|3.0 < media < 6.0|V|
|CE24| media > 6.0|V|

|CT|Valor de Entrada|Resultado Esperado|Classe Equivalência|
|--|--|--|--|
|CT01|-0.01|Valor Inválido|CE01|
|CT02|0|Nota 1 Registrada|CE03|
|CT03|0.01|Nota 1 Registrada|CE03, CE05|
|CT04|9.99|Nota 1 Registrada|CE03, CE05|
|CT05|10|Nota 1 Registrada|CE03|
|CT06|10.01|Valor Inválido|CE02|
|CT07|9.999|Valor Inválido|CE04|
|CT08|-0.01|Valor Inválido|CE06|
|CT09|0|Nota 2 Registrada|CE08|
|CT10|0.01|Nota 2 Registrada|CE08, CE10|
|CT11|9.99|Nota 2 Registrada|CE08, CE10|
|CT12|10|Nota 2 Registrada|CE08|
|CT13|10.01|Valor Inválido|CE07|
|CT14|0.001|Valor Inválido|CE09|
|CT15|0|Valor Inválido|CE11|
|CT10|42.5|Valor Inválido|CE13|
|CT11|32|Carga Horária Salva|CE12, CE14|
|CT12|-3|Valor Inválido|CE15|
|CT13|64|Valor Inválido|CE16|
|CT14|3.5|Valor Inválido|CE18|
|CT15|7|Faltas Registradas|CE17, CE19|
|CT16|2.5, 4.2, 32, 17|Reprovado por Falta|CE20|
|CT17|2.5, 3.2, 32, 7|Reprovado por Média|CE21, CE22|
|CT18|2.5, 4.2, 32, 7|Recuperação|CE21, CE23|
|CT19|6.5, 7.2, 32, 7|Aprovado|CE21, CE24|
