# -Biquadratic-equation
Решение биквадратного уравнония на C# крабометодом
using System;

namespace ConsoleApp1
{
    class Program
    {
        static void Main(string[] args)
        {
            //ввод данных
            Console.WriteLine("Введите первый коэфцициент (А)");
            var A = Console.ReadLine();
            Console.WriteLine("Введите первый коэфцициент (B)");
            var B = Console.ReadLine();
            Console.WriteLine("Введите первый коэфцициент (C)");
            var C = Console.ReadLine();
            while (Int32.TryParse(A, out int j) == false)
            {
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент А");
                A = Console.ReadLine();
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент B");
                B = Console.ReadLine();
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент C");
                C = Console.ReadLine();
                //биквадратное уравнение 
            }
            while (Int32.TryParse(B, out int s) == false )
            {
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент А");
                A = Console.ReadLine();
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент B");
                B = Console.ReadLine();
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент C");
                C = Console.ReadLine();
                //биквадратное уравнение 
            }
            while (Int32.TryParse(C, out int q) == false)
            {
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент А");
                A = Console.ReadLine();
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент B");
                B = Console.ReadLine();
                Console.WriteLine("из-за того что я карб вам придётся ввести всё заново! Введите коэфициент C");
                C = Console.ReadLine();
                //биквадратное уравнение 
            }
            int Anew = Int32.Parse(A);
            int Bnew = int.Parse(B);
            int Cnew = int.Parse(C);
            //считаем само уровнение
            var D = Math.Pow(Bnew, 2)- 4 * Anew * Cnew;
            System.Convert.ToInt32(D);
            if (D < 0)
            {
                Console.ForegroundColor = ConsoleColor.Green;
                Console.WriteLine("Корней уровнения нет!");
            }
            else
            {
                D = Math.Sqrt(D);
                var x1 = (-Bnew - Math.Sqrt(D)) / 2;
                var x2 = (-Bnew + Math.Sqrt(D)) / 2;
                x1 = Math.Pow(x1, 2);
                x2 = Math.Pow(x2, 2);
                Console.ForegroundColor = ConsoleColor.Green; // устанавливаем цвет
                Console.WriteLine($"Корни уровнения {x1} и {x2}");
            }   
        }
        }//проверяем + создаём переменные

        }
