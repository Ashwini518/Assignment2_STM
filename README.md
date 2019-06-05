# Assignment2_STM
STM


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Assignment2
{
    public static class TriangleSolver
    {
        public static string Analyze(int a, int b, int c)
        {
            string result = string.Empty;
            if (a + b > c && b + c > a && c + a > b)
            {
                Console.WriteLine("Given inputs form a triangle.");

                if (a == b && b == c && c==a)
                {
                    result = "Triangle is Equilateral.";
                }
                else if (a == b || b == c || c == a)
                {
                    result = "Triangle is Isosceles.";
                }
                else
                {
                    result = "Triangle is Scalene.";
                }
            }
            else
            {
                 result= "Given inputs doesnot form a triangle.";
            }
            return result;
        }
    }
}
