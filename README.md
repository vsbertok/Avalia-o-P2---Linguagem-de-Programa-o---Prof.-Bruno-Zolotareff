# Avaliacao P2 Linguagem de Programacao Prof. Bruno Zolotareff

Avaliação P2 - 30/05/2026

Dupla:
- Francismar José Haither
- Vitor Souza Bertok

# Máquina de Café com POO. Resposta da pergunta:
- O primeiro paradigma é a Herança, pois quando utilizamos "public class Cafe extends Drink {", estamos herdando da classe abstrata Drink o “sabor” e o “valor” para serem utilizados e aplicados por meio da utilização de vetor e do comando case para definir o menu de escolha do usuário da máquina de café. Dessa forma, manteremos os atributos valor e sabor abstratos na classe Drink, que define o próximo paradigma;
- Abstração: na classe Drink determinados os atributos “valor” (private Double valor;) e “sabor” (private String sabor;) como abstratos, mantendo, dessa forma dados seguros e ocultos, sendo necessário o uso de getters e setters para trazê-los à utilização. Dessa forma, permite que, como já dito, os atributos “sabor” e “valor” abstratos para as demais classes do software, levando ao próximo paradigma;
- Encapsulamento: Ao utilizar os getters e setters dentro da classe drink, da seguinte forma:

  		```
   		(public Drink(String sabor, Double valor); {
          this.sabor = sabor;
          this.valor = valor;
  	      }
  
           // Getters and Setters
           public String getSabor() {
	 	return sabor;
	 	}
  
		public void setSabor(String sabor) {
        this.sabor = sabor;
		```

Estamos encapsulando estes atributos abstratos e setando-os em um novo atributo, público, para ser resgatado nas demais classes utilizadas, neste caso, a classe café.

- E referindo-se ao polimorfismo, poderíamos criar outras classes para outras bebidas, como por exemplo, chás, batidas, etc, utilizando as características da classe drink, ou seja, demais bebidas partindo do princípio da estrutura feita dentro da classe Drink.
Concluímos que, em POO esse paradigma torna possível obter segurança, praticidade, confiabilidade, menores passos para solucionar erros e problemas e, ainda, utilizar atributos protegidos para definir outras classes, sem permitir que seu conteúdo seja divulgado. Um paradigma excelente para trabalhos de programação. 

