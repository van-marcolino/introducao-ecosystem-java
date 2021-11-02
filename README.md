# introducao-ecosystem-java
Estrutura básica de uma declaração de  classe

	package com.dio.base;

	import java.math.BigDecimal;

	public class Order {
			private final String code;
			private final BigDecimal totalValue;

			public Order(String code, BigDecimal totalValue){
				this.code = code;
				this.totalValue = totalValue;}
			public BigDecimal calculateFee(){
		return this.totalValue.multiply(new BigDecimal("0.99"));
			}}

Modificadores de acesso:

public - Qualquer classe de qualquer pacote pode acessar o atributo ou método.

protected - Qualquer classe definida no mesmo pacote ou subclasse.

Sem modificador - aplenas classe definidas no mesmo pacote

provate - Apenas a própria classe

Métodos: funções que definem o comportamento de uma classe.

Construtores: definem como uma classe que será instanciada "construída"

Comum: Definem o comportamento que podem ou não estar atribuídas às regras de negócio. EX: calcular taxas de um pedido, etc.

Condição: Responsável por fazer o desvio do fluxo do código, dependendo da condição.

(if - else) só uma condição
(switch - case) várias condições para a mesma ideia

Repetição: Responsável por executar repetitivamente até que a condição seja satisfeira.

(while)

	int i  =  0;
	while(i <  item.length){
		System.out.println(item[i]);
		i++;
	}
(do - while)
	int i = 0;

	do{
		System.out.println(item[i]);
		i++;
	}while(i <  item.length)
(for)

	for (int =  0; i <  item.length; i++)
	
(enhanced for)

	for( String i : items){
		System.out.println(i);
	}

Comentários em linha: usa o " // ", somente a linha fica em comentário.

Comentários e bloco: começa com " /** " e quando termina de comentatar coloca " */ " .

Javadoc: ferramenta de documentação HTML que se baseia nos comentários do código fonte. Os comentários precisam de tags para que fique legível.

Tags Javadoc: 
@author - especifica o autor da classe ou do método.

@deprecated - identifica classes ou métodos absoletos.

@link - possibilita a definição de um link para um outro documento local ou remoto, usando a URL.

@param - descreve um parâmetro que será passado a um método.

@return - descreve qual o tipo de retorno de um método.

@see - associa a outras classes ou métodos.

@since - descreve desde quando uma classe ou métodos doram adicionados.

@throws - descreve os tipos de exceções que podem ser lançadas por um método.

@version - descreve a versão da classe ou método.
