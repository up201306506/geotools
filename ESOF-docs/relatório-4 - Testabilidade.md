# ESOF - 4º Relatório

22/11/2015

///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

//FALTA FAZER
 
## DEGREE OF TESTABILITY OF THE SOFTWARE PROGRAM

A testabilidade de um software é determinado por factores como:
- controllability;
- observability;
- isolateability;
- separation of concerns;
- understandability;
- heterogeneity.

//FALTA ACABAR

///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

## TEST STATISTICS

1) Number of tests

No GeoTools são apenas exigidos, aquando da submissão de novos módulos, testes unitários JUnit, não são utilizados outros tipos de teste como os testes de desempenho 
e do sistema. 
Não é exigido aos programadores um número específico de testes JUnit, apenas querem que cubra mais de 40% do código desenvolvido.
Não foi possível correr o GeoTools através da ferramenta EclEmma, pelo que não será possível afirmar com toda a certeza a 
quantidade de testes que existem, mas através da análise do código, pode-se dizer que deverá haver mais de 100 testes ao 
longo de todo o programa. Através da documentação disponobilizada também se pode concluir que a cobertura é superior a 
40%.

2) Covarege

Quando é desenvolvido um novo módulo, é exigido ao programador que faça testes JUnit.
Os testes podem ser realizados por uma build box, como por exemplo a hudson, no caso de serem testes online que requerem o uso de serviços Web.
A covertura esperada para a library do GeoTools é de >=40%, através dos testes JUnit.
A cobertura de testes é medida e publicada para a página do Module Matrix.
A cobertura de >=40% é medida por perfil de controlo hudson (hudson control profile). O programador pode fornecer testes de ensaio para que o nightly builds possa correr
contra a base de dados do programador.
Os plugins podem utilizar "conformance test", se disponivel, para alcançar rapidamente os 40%.

3) Code coverage: is it any good?

Uma covertura de 40%, significa que mais de metade do código, não é abrangido pelo conjuntos de testes JUnit, mas este facto não implica que o programa seja melhor
que outro que tenha mais covertura ou que esteja melhor protegido contra bugs, porque é muito fácil aumentar a covertura de um programa, apenas testando os métodos mais
simples.
Uma covertura muito elevada, pode transmitir às pessoas uma falsa segurança, daí ser muito mais importante a qualidade dos testes do que a quantidade. Por exemplo, 
uma covertura de 40%, com poucos testes mas de qualidade, pode ser mais seguro que um software com uma covertura de, por exemplo 70%, com o dobro dos testes do 
primeiro software. 
Para que se concluir que o código é de qualidade, é preciso acrescentar outras técnicas de teste do código, como por exemplo os testes de mutações.
Concluindo, a covertura de um software serve para expor o código que não foi testado pela suite de testes JUnit, e não para verificar a qualidade do código.
Pelos motivos acima referidos, não se pode concluir se a covertura exigida pelo GeoTools, é boa ou não. Pelos dados pode-se concluir que mais de metade do código
do GeoTools não é abrangido pela suite de testes, o que significa que não se pode tirar qualquer conclusão sobre o código não testado. 

## BIBLIOGRAFIA

http://avandeursen.com/2013/11/19/test-coverage-not-for-managers/

http://docs.geotools.org/latest/developer/procedures/supported.html

http://www.ibm.com/developerworks/java/library/j-cq01316/
