1. Projeto CalculadoraPintura - primeiro contato com C# e Microsoft Visual Studio: projeto simples, de cálculo de litragem de tinta para pintar um cômodo, de acordo com os dados ingressados.
2. Projeto Calculadora de Signos - "meu primeiro app em c#" - uso de classes, instaciações e método construtor, try catch
3. Criação de Classe utilizando conceitos de Interface e herança.
4. Tratamento de exceções utilizando os conceitos try, catch, finally, bem como a definição de uma classe customizada que herda da classe geral exception.
5.  Overload: demonstração de como o C# sabe decidir entre o melhor método a invocar.  
6. Delegate: demonstração das formas em que a evocação de métodos pode ocorrer, comentadas, mas com a sintaxe do delegate/event de fato em ação para demonstrar otimização ocorrida.
7. Gerando Classes de Exceptions.
8. Get Read Only: demonstra como utilizar uma classe sem o set para encapsular informações.
9.  EventDelegateInitializer - demonstração de outras formas de usar o delegate initializer, e uma forma mais comum e prática (a que está ativa e não comentada)

lambda debug:

using System.Linq;
using static System.Console;
using static System.Convert;



namespace Exemplo 
{     
    public class Aluno 
    {
        public int Matricula;
        public string Nome;
        public double Mensalidade;
    }

    public static class Repositorio 
    { 
        public static List<Aluno> getAlunos() 
        {
            var lista = new List<Aluno>();
            lista.add(new Aluno() { Matricula = 1, Nome = "Joao1", Mensalidade = 1000 });
            lista.add(new Aluno() { Matricula = 2, Nome = "Joao2", Mensalidade = 1000 });
            lista.add(new Aluno() { Matricula = 3, Nome = "Joao3", Mensalidade = 1300 });
            return lista;
        }
    }
    class Program 
    {
        static void Main(string[] args) 
        {
            var matricula = ReadLine();
            var alunos = Repositorio.getAlunos();
            var aluno = alunos.where(a => a.Matricula == ToInt32(matricula)).FirstOrDefault();
            WriteLine($"O aluno de matrícula {aluno.Matricula} se chama {aluno.Nome}");
        }
    }
}
