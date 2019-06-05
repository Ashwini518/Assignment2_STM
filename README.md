# Assignment2_STM
STM


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using Assignment2;
using NUnit.Framework;

namespace Assignment_2_tests
{
    [TestFixture]
    class Assignment_2_tests
    {
        [Test]
        public void Analyze_ainput6_binput6_cinput12_Outputnotatriangle()
        {
            //Arrange
            int a = 6;
            int b = 6;
            int c = 12;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Given inputs doesnot form a triangle.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
        [Test]
        public void Analyze_ainput12_binput12_cinput12_OutputEquilateral()
        {
            //Arrange
            int a = 12;
            int b = 12;
            int c = 12;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Triangle is Equilateral.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
        [Test]
        public void Analyze_ainput11_binput11_cinput20_OutputIsosceles()
        {
            //Arrange
            int a = 11;
            int b = 11;
            int c = 20;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Triangle is Isosceles.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
        [Test]
        public void Analyze_ainput10_binput18_cinput22_OutputScalene()
        {
            //Arrange
            int a = 10;
            int b = 18;
            int c = 22;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Triangle is Scalene.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);

        }
        [Test]
        public void Analyze_ainput12_binput12_cinput24_Outputnotatriangle()
        {
            //Arrange
            int a = 12;
            int b = 12;
            int c = 24;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Given inputs doesnot form a triangle.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
        [Test]
        public void Analyze_ainput100_binput100_cinput100_OutputEquilateral()
        {
            //Arrange
            int a = 100;
            int b = 100;
            int c = 100;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Triangle is Equilateral.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
        [Test]
        public void Analyze_ainput120_binput99_cinput120_OutputIsosceles()
        {
            //Arrange
            int a = 120;
            int b = 99;
            int c = 120;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Triangle is Isosceles.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
        [Test]
        public void Analyze_ainput300_binput306_cinput200_OutputScalene()
        {
            //Arrange
            int a = 300;
            int b = 306;
            int c = 200;
            string res = TriangleSolver.Analyze(a, b, c);
            string expectedoutput = res;

            //Act
            string actualresult = "Triangle is Scalene.";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);

        }

    }
}
