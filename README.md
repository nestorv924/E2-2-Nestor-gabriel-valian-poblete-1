using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Diagnostics;

namespace fibonacci
{
    class Program
    {
        public int t, nu, n, i=0, ex;
       
        public void Fub()
        {
            t = 0;
            nu = 1;
            Console.WriteLine(Cuantos numeros fibonacci deseas ?");

            n = int.Parse(Console.ReadLine());
            
            Console.WriteLine("");
            for (i = 0; i < n; i++)
            {
                e = t;
                t = nu;
                nu= ex+ t;
                Console.WriteLine(temporal);
            }
        }

        static void Recursividad(int x)
        {
            Console.WriteLine("  ");
            Console.WriteLine(" 10 Numeros para fibonacci");

            Console.WriteLine(" ");
            Console.WriteLine(" ");

            int te, num, i1=0, ext;
            te = 0;
            num = 1;

                for(i1=0; i1<x;i1++)
                {
                    ext=te;
                    te=num;
                    num = ext + te;
                    Console.WriteLine(te);
                }

        }


        static void Main(string[] args)
        {
            {
                Program obj= new Program();

                
                Stopwatch stopWatch = new Stopwatch();

                stopWatch.Start();
                obj.Fubonacci();
                stopWatch.Stop();

                Console.WriteLine("proceso en finalizado en: " + stopWatch.Elapsed.ToString(), "mensaje es sistema");

                
                Stopwatch stopWatch1 = new Stopwatch();
                stopWatch1.Start();
                Recursividad(10);
                stopWatch1.Stop();
                Console.WriteLine("proceso  finalizado en: " + stopWatch1.Elapsed.ToString(), "Mensaje es Sistema");
                Console.ReadKey();

            }
        }
    }
}
