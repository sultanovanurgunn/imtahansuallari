# imtahansuallari
#sual1
using System;

class Program
{
    static void Main()
    {
        // Dəyişənləri şərtdəki kimi sadə şəkildə təyin edirik
        double x = 1.0;  // x0 = 1
        double xn = 2.0; // xn = 2
        double dx = 0.05; // Delta x = 0.05

        Console.WriteLine("x qiyməti -- v(x) qiyməti");
        Console.WriteLine("-----------------------");

        // x dəyişəni 2-dən kiçik və ya bərabər olduğu müddətcə dövr edir
        while (x <= xn)
        {
            // Riyazi düsturu birbaşa yazırıq
            double vx = Math.Sqrt(10 * x) + Math.Sin(Math.Abs(x - 6.25));

            // Ən sadə şəkildə ekrana çıxarırıq
            // sətirdəki $ işarəsi dəyişənləri birbaşa mətnin içində {x} kimi yazmağa icazə verir
            Console.WriteLine($"x = {x}  -->  v(x) = {vx}");

            // x-in qiymətini hər addımda 0.05 artırırıq
            x += dx;
        }
    }
}
