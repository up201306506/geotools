# GeoTools

Development Requirements

Para o Geotools funcionar são necessários dois programas em específico. Um deles é o Apache Maven (versão 3.2.1) que é uma ferramenta de compilação utilizada primariamente em projetos Java. O outro é Java 2 Software Developers Kit (Java 7) que é uma plataforma utilizada para desenvolver projetos com a linguagem Java.



Elicitation
	Tal como ocorre com o reportar de erros, os pedidos de novas funcionalidades do geotools é feito atravéz do Issue Tracker JIRA. É possivel encontrar especificamente apenas os pedidos de funcionalidades atravez da filtragem em New Feature, Improvement e Task e finalmente, marcar apenas problemas em estado aberto ‘Open’.
	Em alternativa, há sempre a possibilidade de comunicar para uma das mailing lists do projecto, sendo que outrem poderá abrir uma Issue no tracker se a sugestão for relevante.

Specification, Analysis
	Qualquer pessoa pode fazer uma request e qualquer pessoa pode participar da discussão. O tracker tem uma secção de atividade que incorpora essa vertentes. 
       Os pedidos devem 
Validation
	No final, todas as alterações devem ser feitas por pull request atravéz do github. Os próprios pull request tem as suas regras, incluindo referência cruzada com o issue no JIRA, test cases e. No JIRA é possivel encontrar quem é ou foi o responsável ‘Assignee ‘ pelo problema marcado.
Dependendo da alteração, o grupo de utilizadores que tem a responsabilidade de a desenvolver ocorre de forma hierarquica  consoante o guia de contribuição ( Contributors < Commiters < Module Maintainers). Mas mesmo feito um Pull Request, não é garantido que o problema seja acrescentado a master até ser feita a sua validação. Quando o Module Maintainer sentir que o seu módulo está pronto, pode decidir declará-lo formalmente supported, momento esse em que o módulo é transferido para o directório modules/plugin/ ou modules/extension/.
