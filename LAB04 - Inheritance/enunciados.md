# Exercício de herança

# Ex01 

**não utilizar herança no ex01**

Relembre o exercício da prática anterior. Nele indicamos que as figurinhas da copa são compostas pelas seguintes informações sobre os jogadores: Nome do Jogador, Data de Nascimento, Altura, Peso, Posição, País. Todos criaram a classe Figurinha, que continha todas as informações das figurinhas. Modifique o exercício para que inclua um construtor que inicialize todos os atributos. Crie também na classe um métodos MostrarFigurinha(), que imprime na tela todos os dados da Figurinha.

Agora crie a classe para as figurinhas extras. Essas são bem mais raras e não fazem parte da coleção regular, sendo caracterizadas como uma coleção à parte. Além de todos os atributos das figurinhas regulares, as raras são divididas em duas categorias, "Legends" e "Rookies", e possuem quatro variações de cor: bordô, bronze, prata e ouro". Crie uma classe chamada ex01.ex02.ex03.FigurinhaExtra, que contenha todos atributos da classe Figurinha e acrescente os dois novos atributos. Utilize boas práticas de POO (atributos privados, métodos get/set), crie um construtor que inicializa todos os parâmetros e crie também o método MostrarFigurinha().

Faça um programa principal que cria uma Figurinha e uma ex01.ex02.ex03.FigurinhaExtra, e mostre os dados das figurinhas criadas

# Ex02
O conceito de herança (inheritance) em POO é muito utilizado para reaproveitamento de código.

- Modifique a classe Figurinha, transformando os atributos *private* para *protected*
- Modifique a classe ex01.ex02.ex03.FigurinhaExtra, eliminando todos os atributos e métodos reduntantes de Figurinha. Obtenha os valores desses atributos por herança utilizando a palavra chave *extends*, isto é: "public class ex01.ex02.ex03.FigurinhaExtra extends Figurinha {".
- Note que a herança irá trazer os atributos e os métodos para a classe ex01.ex02.ex03.FigurinhaExtra.
- Note que o método MostrarFigurinha() deve continuar em ex01.ex02.ex03.FigurinhaExtra, pois ele é diferente do método ex01.ex02.ex03.FigurinhaExtra() da classe Figurinha
- O construtor deve ser modificado, de forma a inicializar somente os atributos de ex01.ex02.ex03.FigurinhaExtra. Os atributos que são originais de classe Figurinha (chamada de superclasse ou classe mãe/pai) deverão ser inicializados por meio da chamada do construtor original de Figurinha. Isso é feito usando a palavra reservada *super*

Faça um programa principal que cria uma Figurinha e uma ex01.ex02.ex03.FigurinhaExtra, e mostre os dados das figurinhas criadas

# Ex03
- Modifique a classe Figurinha, transformando os atributos *protected* para *private*
- Entenda o erro que ocorre em MostrarFigurinha() da classe ex01.ex02.ex03.FigurinhaExtra com essa modificação
- Modifique o método MostrarFigurinha() para ser possível vizualizar os atributos privados de Figurinha. Para isso use *super.MostrarFigurinha()*
- Crie um novo construtor, que terá como parâmetro uma Figurinha (normal) e os dois atributo adicionais de ex01.ex02.ex03.FigurinhaExtra. Esse construtor permitirá criar um novo objeto de ex01.ex02.ex03.FigurinhaExtra a partir de um objeto já existente de Figurinha (ou seja, uma figurinha extra de um jogador que já foi criado)

Faça um programa principal que cria uma Figurinha e uma ex01.ex02.ex03.FigurinhaExtra, e mostre os dados das figurinhas criadas

# Ex04
Teste de chamada de herança
 Faça um programa que contenha três classes: ex04.C1; ex04.C2; ex04.C3

- A classe ex04.C1 é base da Classe ex04.C2, que por sua vez é base da Classe ex04.C3
- Para cada classe, inclua um atributo público, protegido e privado (pode ser de qualquer tipo)
- Para cada classe, construa um construtor padrão sem parâmetros e um construtor com parâmetros
- Nos construtores de cada classe, inclua um comando que imprime uma mensagem indicando a passagem pelo contrutor. Por exemplo, para ex04.C1:
  "Classe ex04.C1: chamada do construtor padrao, sem parametros"
  "Classe ex04.C3: chamada do construtor com parametros"
- Na classe ex04.C3 inclua um construtor que use o "super" para chamar o construtor da classe ex04.C2 com parâmetro
- Em todas as classes, inclua um método que chama mostar_atributos, que mostra os valores de *todos* os atributos de um objeto (não utilizar *super*)
    - Lembre que as classes herdam os atributos, inclusive os privados - e esses também devem ser mostrados 
- Em todas as classes, inclua um método que chama mostar_atributos_super, que mostra os valores de *todos* os atributos de um objeto e que utilize *super*

# Ex05
Uma ex05.empresa tem quatro tipos de funcionários: chefes, vendedores, operários e horistas. Cada um desses funcionários ganha seus salários conforme regras distintas, apresentadas a seguir: 

ex05.Chefe: salário fixo e predefinido;
ex05.Vendedor: valor fixo + comissão * vendas;
ex05.Operario: valor por produção * quantidade produzida;
ex05.Horista: valor por hora * total de horas trabalhadas.


Crie as classes correspondentes, adicionando atributos e métodos que achar necessários. A classe *ex05.Funcionario* deve incluir os campos privados *nome*, *dataNascimento* e *salario*. Além disso, crie uma classe *Empresa*, que conterá o método *ex01.ex04.main()*. A ex05.empresa tem vários funcionários, logo crie um vetor (array) para cada tipo de funcionário, instancie no mínimo 2 exemplos de cada tipo de funcionário. Mostre uma chamada para cálculo do salário

# Ex06
Crie uma classe chamada {ex06.Ingresso}, que possui um valor e um método {escreveValor()}. Em seguida:

Crie uma classe {ex06.VIP}, que herda {ex06.Ingresso} e possui um valor adicional. Crie um método que retorne o valor do ingresso ex06.VIP (com o adicional incluído).
	
Crie uma classe {ex06.Normal}, que herda {ex06.Ingresso} e possui um método que imprime: "ex06.Ingresso ex06.Normal".
	
Crie uma classe {ex06.CamaroteInferior} (que possui a localização do ingresso e métodos para acessar e imprimir esta localização) e uma classe {ex06.CamaroteSuperior}, que é mais cara (possui valor adicional). Esta última possui um método para retornar o valor do ingresso. Ambas as classes herdam a classe {ex06.VIP}.
