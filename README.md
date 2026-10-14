using System;
 class program
{
    static int Suma(int n)
    {
        if (n <=0)
        return 0;
        return n + Suma(n - 1);
    }
    static void Main()
    {
        Console.WriteLine("Ingrese el Número: ");
        int n = int.Parse(Console.ReadLine());

        if (n < 0 || n > 10000)
        {
            Console.WriteLine("Ingrese un numero entre 1 a 10,000");
            return;

        }
        Console.WriteLine("La suma es: " + Suma(n));
    }
}
