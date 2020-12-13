# DESIGN PATTERNS

Este reposótorio contém algumas informações sobre os principais Design Patterns existentes, estas infos foram tiradas do curso Design Patters by @alura.

--- 

## Strategy:
O Strategy nos oferece uma maneira flexível para escrever diversos algoritmos diferentes, e de 
passar esses algoritmos para classes clientes que precisam deles. Esses clientes desconhecem qual é o algoritmo "real" 
que está sendo executado, e apenas mandam o algoritmo rodar. Isso faz com que o código da classe cliente fique bastante 
desacoplado das implementações concretas de algoritmos, possibilitando assim com que esse cliente consiga trabalhar 
com N diferentes algoritmos sem precisar alterar o seu código.

---

## Chain of Responsability:
O padrão Chain of Responsibility cai como uma luva quando temos uma lista de comandos 
a serem executados de acordo com algum cenário em específico, e sabemos também qual o próximo cenário que deve ser 
validado, caso o anterior não satisfaça a condição.

---

## Template Method:
Quando temos diferentes algoritmos que possuem estruturas parecidas, o Template Method é 
uma boa solução. Com ele, conseguimos definir, em um nível mais macro, a estrutura do algoritmo e deixar "buracos", 
que serão implementados de maneira diferente por cada uma das implementações específicas.

---

## Decorator: 
Sempre que percebemos que temos comportamentos que podem ser compostos por comportamentos de outras 
classes envolvidas em uma mesma hierarquia, como foi o caso dos impostos, que podem ser compostos por outros impostos. 
O Decorator introduz a flexibilidade na composição desses comportamentos, bastando escolher no momento da instanciação, 
quais instancias serão utilizadas para realizar o trabalho.

---

## State:
A principal situação que faz emergir o Design Pattern State é a necessidade de implementação de uma máquina de estados.
Geralmente, o controle das possíveis transições são vários e complexos, fazendo com que a implementação não seja simples. 
O State auxilia a manter o controle dos estados simples e organizados através da criação de classes que representem 
cada estado e saiba controlar as transições.

---

## Builder:
Sempre que tivermos um objeto complexo de ser criado, que possui diversos atributos, 
ou que possui uma lógica de criação complicada, podemos esconder tudo isso em um Builder.

---

## Observer: 
Quando o acoplamento da nossa classe está crescendo, ou quando temos diversas ações diferentes 
a serem executadas após um determinado processo, podemos implementar o Observer. Ele permite que diversas ações 
sejam executadas de forma transparente à classe principal, reduzindo o acoplamento entre essas ações, facilitando
a manutenção e evolução do código.

---

## Factory:
Instancia uma classe que é importante/complexa, e seu processo de criação deve ser isolado.
Usamos uma fábrica quando temos que isolar o processo de criação de um objeto em um único lugar. Essa fábrica pode descobrir 
como criar o objeto dentro dela própria, mas geralmente ela não precisa de muitas informações para criar o objeto.

---

## Flyweight:
Serve para quando temos muitas instâncias do mesmo objeto andando pelo sistema, e 
precisamos economizar. Para tal, o Flyweight faz uso de uma fábrica modificada, que guarda essas instâncias.
Diferenca do Singleton Vs Flyweight: A diferença é que o Flyweight garante que existam apenas uma única instância de vários elementos. 
É um "singleton maior".

---

## Memento:
Serve para armazenar os estados dos objetos, porém pode ocupar uma grande quantidade de memória, o melhor seria não
armazenar todo objeto e sim as propriedades que mais fazem sentido.

---

## Interpreter:
É geralmente útil para interpretar DSLs (se você não sabe o que é uma DSL, pode ler mais sobre 
isso aqui: http://pt.wikipedia.org/wiki/Linguagem_de_dom%C3%ADnio_espec%C3%ADfico. É comum que, ao 
ler a string (como por exemplo 2+3/4), o programa transforme-o em uma melhor estrutura 
de dados (como as nossas classes Expressao) e aí interprete essa árvore.

---

## Visitor:
Quando temos uma árvore, e precisamos navegar nessa árvore de maneira organizada.

---

## Bridges:
Hoje temos muitos serviços similares que são prestados por diferentes empresas, criamos uma interface para 
servir de ponte para uma implementação concreta.

---

## Adapters:
Quando temos um conjunto de classes legadas, que achamos que seu uso vai sujar o novo sistema, 
criamos um "adaptador" que facilita sua utilização. O nome desse padrão de projetos é Adapter

---

## Commander:
Usamos ele quando temos que separar os comandos que serão executados do objeto que ele pertence. 
Um bom exemplo disso é o uso de filas de trabalho.

---

## Facedes:
Essa classe provê acesso a todos os outros sub-sistemas, é bem comum também que 
não haja mais de uma instância dessa classe espalhada pelo sistema.

---

## Singleton:
Ele faz com que só exista uma única instância da classe em todo o sistema!

---

Developed by Bruno Lima Dec/2020 🦧
