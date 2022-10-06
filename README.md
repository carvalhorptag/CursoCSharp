CursoCSharp
using System
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CursoSCharp.Colecoes 
{
    public class Produto 
    {
        public string Nome;
        public double Preco;

        public Produto(string nome, double preco) 
        {
            Nome = nome;
            Preco = preco;

        }
    }
    internal class ColecoesList 
    {
public static void Executar() 
        {
            var livro = new Produto("Game of Throne", 49.9);

            var carrinho = new List<Produto>();
            carrinho.Add(livro);

            var combo = new List<Produto> 
            {
                new Produto("Camisa",29.9),
                new Produto("8ª Temporada Game of Throne", 99.9),
                new Produto("Poster", 10)
            };
            carrinho.AddRange(combo);
            Console.WriteLine(carrinho.Count);
            
        }
    }
}
