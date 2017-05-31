# Problem.X
softuni Homework
using System;

namespace Homework
{
    class Program
    {
        static void Main()
        {
            int n = int.Parse(Console.ReadLine());
            int a = 0;
            if (n % 2 == 0)
            {
                a = (n / 2) - 1;
            }else
            {
                a = (n - 1) / 2;
            }
            for (int i = 0; i < a; i++)
            {
                Console.WriteLine("{0}x{1}x{0}",new string(' ',i),new string
                    (' ',(n-2)-(i*2)));
            }
            Console.WriteLine("{0}x{0}",new string(' ',a));
            for (int i = a; i > 0; i--)
            {
                Console.WriteLine("{0}x{1}x{0}",new string(' ',i-1),
                    new string(' ',(n)-(i*2)));

            }
        }
    }
}
