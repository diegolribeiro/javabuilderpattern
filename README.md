# Exemplo do pattern Builder

Pattern Builder é um pattern criacional, ou seja, utilizado para criar objetos de uma classe.

Ele é muito utilizado com classes imutáveis. 

Classe imutável é uma classe que seu estado e suas propriedades não podem ser alterados depois de criado. Quando você trabalhar com classes imutáveis é normal o construtor ter diversos parâmetros 
no qual você é responsável de prover os valores, sem uma documentação consistente trabalhar com construtor com muitos parâmetros é ruim, e considerado uma má prática.

Além disso a montagem de um objeto pode conter outros objetos complexos dentro dela dificultando ainda mais a criação.
São em situações parecidas com essa que o design pattern builder é utilizado:
•	Quando temos um complexo processo de construir um objeto que envolve múltiplos passos.
•	No builder no removemos a lógica relacionado a construção do objeto do código do "cliente" e abstraímos em classes separadas.


Algumas Regas que podem ajudar na implementação do builder
1.	Primeiro estudar o objeto que precisa ser criado, entender do que esse objeto é composto, qual a lógica para cria-lo, quais os steps, analise os construtores das classes envolvidas  
2.	Pensar em como prover o método de montagem do objeto
3.	Pensar em prover um caminho para disponibilizar o objeto construído.
4.	Um diretor pode ser uma classe separada ou o cliente pode fazer o papel de diretor
