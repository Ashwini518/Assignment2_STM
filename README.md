# Assignment2_STM
STM


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Assignment2
{
    class Program
    {
        static void Main(String[] args)
        {
            string givenInput = "";
            bool validMenu = false;
            string d = string.Empty;
            while (validMenu == false)
            {
                Console.WriteLine("1=Enter Triangle dimensions");
                Console.WriteLine("2 = Exit \n");

                Console.WriteLine("Please select an option, by entering a number:\n");
                givenInput = Console.ReadLine();
                if (givenInput != "1" &&
                    givenInput != "2")
                {
                    Console.WriteLine("That's not a valid menu option, please try again:\n");
                }
                else if (givenInput == "1")
                {
                    Console.WriteLine("Enter three sides of traingle :");
                    Console.WriteLine("Enter First side of triangle : ");
                    int a = int.Parse(Console.ReadLine());
                    Console.WriteLine("Enter Second Side of traingle : ");
                    int b = int.Parse(Console.ReadLine());
                    Console.WriteLine("Enter Third Side of traingle : ");
                    int c = int.Parse(Console.ReadLine());
                    d = TriangleSolver.Analyze(a, b, c);
                    Console.WriteLine("{0}", d);
                }
                else
                {
                    validMenu = true;
                    break;

                }

            }
        }
    }
}
