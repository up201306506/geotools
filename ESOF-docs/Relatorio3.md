ESOF - 3º Relatório


#Introdução

###Sendo o Geotools uma biblioteca open source de Java, perceber a sua arquitetura ajuda quando se pretende organizar bem uma aplicação a que use o Geotools.


#Arquitetura

<img src="./images/geotools_arquitetura.png" />

###A arquitetura usada pelo Geotools funciona como uma “stack”. Tem várias camadas e cada uma destas é acrescentada a cima das outras já existentes. Cada uma destas camadas interage com as outras de várias formas. Por exemplo, a parte dos plugins precisa de várias camadas para funcionar como por exemplo a data na zona da implementação.

###O geotools também disponibiliza extensões , mas estas funcionam independentemente do resto.

<img src="./images/geotools_arquitetura_extensões.png" />


###Como o geotools é uma biblioteca e não uma aplicação, esta é das poucas informações que temos em relação à sua arquitetura. Se tivessemos que escolher um tipo de arquitetura para o Geotools seria o “Layered Architecture”.
