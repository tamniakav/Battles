# Battles
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Battles
{
    class Battles
    {
        static void Main(string[] args)
        {
            int playerOne = int.Parse(Console.ReadLine());
            int playerTwo = int.Parse(Console.ReadLine());
            int battles = int.Parse(Console.ReadLine());
            int counter = 0;

            for (int i = 1; i <= playerOne; i++)
            {
                for (int j = 1; j <= playerTwo; j++)
                {
                    Console.Write($"({i} <-> {j}) ");
                    counter++;
                    if (counter == battles)
                    {
                        break;
                    }
                }
                if (counter == battles)
                {
                    break;
                }
            }
            Console.WriteLine();
        }
    }
}
