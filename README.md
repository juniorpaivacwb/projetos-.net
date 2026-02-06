1. Projeto CalculadoraPintura - primeiro contato com C# e Microsoft Visual Studio: projeto simples, de cálculo de litragem de tinta para pintar um cômodo, de acordo com os dados ingressados.
2. Projeto Calculadora de Signos - "meu primeiro app em c#" - uso de classes, instaciações e método construtor, try catch
3. Criação de Classe utilizando conceitos de Interface e herança.
4. Tratamento de exceções utilizando os conceitos try, catch, finally, bem como a definição de uma classe customizada que herda da classe geral exception.
5.  Overload: demonstração de como o C# sabe decidir entre o melhor método a invocar.  
6. Delegate: demonstração das formas em que a evocação de métodos pode ocorrer, comentadas, mas com a sintaxe do delegate/event de fato em ação para demonstrar otimização ocorrida.
7. Gerando Classes de Exceptions.
8. Get Read Only: demonstra como utilizar uma classe sem o set para encapsular informações.
9.  EventDelegateInitializer - demonstração de outras formas de usar o delegate initializer, e uma forma mais comum e prática (a que está ativa e não comentada)
10. Lambda Debbuging: dado o código, colocado um breaking point na linha 35, e observado os retornos do processamento na janela Watch. Utilizada também a janela Imediata, para testar novas expressões lambda para ver como o sistema se comporta. Ação útil para trazer soluções e apontar direções no dia a dia.
11. Layout - utilização da definição de Layouts no Visual Studio, podendo trazer com agilidades janelas salvas em diferentes formatos que melhor se encaixem a diferentes momento de programação, podendo ser acessados pelo menu Janelas, ou fixados na barra de tarefa. Útil para trabalho e equipe que compartilham o mesmo computador, e cada programador tem autonomia para configurar o ambiente da maneira que lhe é mais produtiva.
12. QuickActions / Refactoring (CalculadoraRefactoring) - utilização, mesmo que não aparente porque ocorre durante o desenvolvimento no IDE, de quick actions, para alterar nome de métodos, criação de classes, inserção de "using" por sugestão e guia das quick actions.
13 . Alocação de Memória no tipo Value e do Tipo Reference (ValueRef) - entendendo como são reservados valores na memória quando passados um tipo value, tipo que gera uma marcação na memória, e um tipo refence, que pode apontar para vários espaços na memória.
14. Alocação de Memória no tipo Value e do Tipo Reference (ValueReference) - parecido com o item 13, porem com uma classe herdando de Object para utilizar ToString (para fazer o compilador interpretar corretamente quais parâmetros ele deve converter em String e trazer na tela), e Equals.
15. Assessores e Propriedades (AssessorePropriedades) - usando enum para limitar valores que variáveis podem receber, explicitando a diferença entre Class (tipo reference quepode trabalhar com ponteiros, onde diferentes variáveis do tipo da referida class podem apontar para a mesma estrutura de memória, e Struct (tipo Value cujas varáveis a ele atribuidas não apontam para a mesma estrutura de memória, porém criam uma cópia e passam a ter a própria estrutura de memória separada).
16. Construtores e Overloads (ContrutoreseOverloads) - aborda de maneira prática o uso de Construtores, e o Overloads que cada Construtor pode ter, baseado na quantidade de atributos que recebem, precisando nesse sentido ter um identidade única. Aborda também o uso de ":base", explicitando que ainda que um classe herde de uma Classe pai com diversos construtores, é necessário indicar com o uso de ":base" quais atributos serão passados para a classe filha.
17. GetSet (GetSet) - apresenta forma tradicional e C# para encapsular dados sensíveis usando, construtor, get e set.
18. Propriedades (AssessoresPropriedades) - declaradas variáveis públicas inicialmente, e depois utilizada a QuickAction de encapsulamento, onde o Visual Studio gerou automaticamente as propriedades Get e Set e tornou as variáveis em Private. Dessa forma apesar do Main invocar nomes que parecem de variável, na verdade invoca métodos com Propriedades que encapsulam as informações, como pede as boas práticas. Usada tamvbém técnica de personalização de Exception.





