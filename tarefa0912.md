## Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência.

**DEFINIÇÃO**:
1. Definir um conjunto de classes de Equivalência e um conjunto de casos de testes derivados, para testar a seguinte função de avaliação universitária.
2. A função avalicao, recebe como parâmtros os seguintes dados:
   2.1. **nota1** (numérico de ponto flutuante com duas casas decimais);
   2.2. **nota2**  (numérico de ponto flutuante com duas casas decimais);
   2.3. **cargaHoraria** (numérico inteiro, positivo);
   2.4. **faltas** (numérico inteiro, positivo).
3. A forma de calcular a avaliação é a seguinte:
  3.1. Se a quantidade de faltas for superior a 25% da carga horária, o aluno estará reprovado por falta. Neste caso a função retorna a seguinte mensagem "Reprovado por Falta";
  3.2. Estando o aluno reprovado por falta, não haverá a necessidade de se avaliar as notas;
  3.2. Se a média entre nota1 e nota2 for menor que 3.0, o aluno estará reprovado por média.  Neste caso a função retorna a seguinte mensagem "Reprovado por Média";
  3.3. Se a média entre nota1 e nota2 for >= 3.0 e < 6.0, o aluno estará em recuperação.  Neste caso a função retorna a seguinte mensagem "Recuperação";
  3.4 Em qualquer outra situação o aluno estará  aprovado. Então a função retornará a mensagem: "Aprovado".
4. O Conjunto de classes de Equivalência deverá ser definido seguindo o seguinte padrão:

|id|descrição|V/I|
|--|--|--|
|CE01|nota1 < 0|I|

Onde:
**CE** = Classe de Equivalência, seguido de um número sequencial;
**Descrição** = define um cenário de teste;
**V/I** = Válida ou Inválida.

5. O Conjunto de casos de testes derivado das classes de Equivalência deve seguir o seguinte padrão:

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
2. Local de Entrega: A entrega deverá seu repositório pessoal, utilizado para a manutenção dos artefatos de trabalho d disciplina (ts-2021-2);
3. Data da Entrega: Esta tarefa deve estar disponível para avaliação até o dia 28/12/2021 às 23h59min.
4. Critério de Aceitação: tarefa entregue conforme especificado e na data definida.
5. Caso necessite de suporte, pode encaminhar mensagem para o professor.

RESOLUÇÃO:
| id |                descrição                |V/I|
|----|-----------------------------------------|---|
|CE01|nota1 < 0                                | I |
|CE02|nota1 > 10                               | I |
|CE03|0 < nota1 < 10                           | V |
|CE04|nota1 tem mais que duas casas decimais   | I |
|CE05|nota1 tem duas ou menos casas decimais   | V |
|CE06|nota2 < 0                                | I |
|CE07|nota2 > 10                               | I |
|CE08|0 < nota2 < 10                           | V |
|CE09|nota2 tem mais que duas casas decimais   | I |
|CE10|nota2 tem exatamente duas casas decimais | V |
|CE11|cargaHoraria < 1                         | I |
|CE12|cargaHoraria >= 1                        | V |
|CE13|cargaHoraria tem casas decimais          | I |
|CE14|cargaHoraria é número inteiro            | V |
|CE15|faltas < 0                               | I |
|CE16|faltas > cargaHoraria                    | I |
|CE17|0 <= faltas <= cargaHoraria              | V |
|CE18|faltas tem casas decimais                | I |
|CE19|faltas é número inteiro                  | V |
|CE20|faltas > cargaHoraria * 0.25             | V |
|CE21|faltas < cargaHoraria * 0.25             | V |
|CE22|media < 3.0                              | V |
|CE23|3.0 < media < 6.0                        | V |
|CE24| media > 6.0                             | V |

| CT |Valor de Entrada| Resultado Esperado |Classe Equivalência|
|----|----------------|--------------------|-------------------|
|CT01|-2              |Valor Inválido      |CE01               |
|CT02|13.1            |Valor Inválido      |CE02               |
|CT03|6.753           |Valor Inválido      |CE04               |
|CT04|7.3             |Nota 1 Registrada   |CE03, CE05         |
|CT05|-4.3            |Valor Inválido      |CE06               |
|CT06|11              |Valor Inválido      |CE07               |
|CT07|3.667           |Valor Inválido      |CE09               |
|CT08|5               |Nota 2 Registrada   |CE08, CE10         |
|CT09|0               |Valor Inválido      |CE11               |
|CT10|42.5            |Valor Inválido      |CE13               |
|CT11|32              |Carga Horária Salva |CE12, CE14         |
|CT12|-3              |Valor Inválido      |CE15               |
|CT13|64              |Valor Inválido      |CE16               |
|CT14|3.5             |Valor Inválido      |CE18               |
|CT15|7               |Faltas Registradas  |CE17, CE19         |
|CT16|2.5, 4.2, 32, 17|Reprovado por Falta |CE20               |
|CT17|2.5, 3.2, 32, 7 |Reprovado por Média |CE21, CE22         |
|CT18|2.5, 4.2, 32, 7 |Recuperação         |CE21, CE23         |
|CT19|6.5, 7.2, 32, 7 |Aprovado            |CE21, CE24         |