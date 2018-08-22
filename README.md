//# Sum-of-numbers
//Just recieving input to sum total of 10 numbers
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Sum_of_Numbers
{
    class Program
    {
        static void Main(string[] args)
        {
            double sum=0;
            Console.WriteLine("Here you will sum the addition of any digits ranging from 0 - 100.");
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine("Please enter your digit(s): ");
                double a = Convert.ToDouble(Console.ReadLine());
                if ((a < 0) || (a > 100))
                {
                    Console.WriteLine("Digit(s) entered, out of range. Please enter a digit(s) ranging between 0 and 100");
                    --i;
                }
                else
                {
                    sum = sum + a;
                }
            }
            Console.WriteLine($"Your total sum is {sum}");
            Console.ReadKey();
        }
    }
}
