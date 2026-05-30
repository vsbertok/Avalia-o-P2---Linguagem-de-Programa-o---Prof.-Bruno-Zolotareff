# Avaliação P2 Linguagem de Programação Prof. Bruno Zolotareff

Avaliação P2 - 30/05/2026

Dupla:
- Francismar José Haither
- Vitor Souza Bertok

# Máquina de Café com POO. Resposta da pergunta:

Herança: O primeiro paradigma é a Herança. Ao utilizarmos `public class Cafe extends Drink`, estamos fazendo com que a classe `Cafe` herde os atributos e métodos da classe mãe (`Drink`). Isso evita a repetição de código, pois características comuns a todas as bebidas (como `sabor` e `valor`) são escritas apenas uma vez, sendo reaproveitadas por todas as classes filhas que a máquina de café vier a ter.

Abstração: A Abstração consiste em focar nas características essenciais do objeto, ignorando detalhes menos importantes. Ao criarmos a classe `Drink`, criamos um "molde" conceitual para qualquer bebida. A máquina de café não prepara uma "Bebida" genérica, ela prepara um "Café" específico. A abstração nos permite definir que toda bebida terá uma forma de ser preparada, deixando os detalhes exatos de como isso é feito para as classes específicas.

Encapsulamento: O Encapsulamento garante a segurança e a integridade dos dados da nossa aplicação. Na classe `Drink`, definimos os atributos `sabor` e `valor` como privados (`private`). Com isso, impedimos que eles sejam acessados ou modificados diretamente por outras partes do código. Para permitir a interação segura com esses atributos, criamos métodos públicos (getters para ler a informação e setters para alterá-la), da seguinte forma:

```java
public Drink(String sabor, Double valor) {
    this.sabor = sabor;
    this.valor = valor;
}

// Getters and Setters
public String getSabor() {
    return sabor;
}

public void setSabor(String sabor) {
    this.sabor = sabor;
}
```

Polimorfismo: Por fim, o Polimorfismo (que significa "várias formas") é o que nos dá flexibilidade. Se criarmos outras classes como `Cha` ou `ChocolateQuente` (que também herdam de `Drink`), o polimorfismo nos permite tratar todas elas de forma padronizada. Por exemplo, a máquina de café pode acionar um método `prepararBebida()` e, graças ao polimorfismo, o programa saberá exatamente como agir dependendo do tipo de objeto escolhido pelo usuário no menu (um café será preparado de um jeito, e um chá de outro), mesmo usando o mesmo comando básico. 

