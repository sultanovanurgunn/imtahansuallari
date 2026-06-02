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
#sual2
using System;

class Program
{
    static void Main()
    {
        // Şəkildə verilən bütün qiymətləri sadə dəyişənlər olaraq təyin edirik
        double x = 1.0;     // x0 = 1
        double xn = 2.3;    // xn = 2.3
        double dx = 0.1;    // Delta x = 0.1
        double a = 5.0;     // a = 5
        double b = 2.1;     // b = 2.1

        Console.WriteLine("x qiymeti -- y(x) qiymeti");
        Console.WriteLine("-----------------------");

        // x dəyişəni 2.3-dən kiçik və ya bərabər olduğu müddətcə dövr davam edir
        while (x <= xn)
        {
            // Düsturu tam sadə şəkildə hesablayırıq
            // Math.Exp(a * x) ifadəsi e üstü (a vurulsun x) deməkdir
            double yx = Math.Exp(a * x) - Math.Exp(b * x);

            // Öyrəndiyimiz ən sadə üsulla ekrana çıxarırıq
            Console.WriteLine($"x = {x}  -->  y(x) = {yx}");

            // x-in qiymətini hər addımda 0.1 artırırıq
            x += dx;
        }
    }
}
#sual3
using System;

class Program
{
    static void Main()
    {
        // Şəkildə verilən ilkin qiymətləri təyin edirik
        double x = 1.0;          // x0 = 1
        double xn = 41.0;        // xn = 41
        double dx = 5.0;         // Delta x = 5
        double a = 3.0;          // a = 3
        
        // t = kök altında 7
        double t = Math.Sqrt(7); 

        Console.WriteLine("x qiymeti -- z(x) qiymeti");
        Console.WriteLine("-----------------------");

        // x dəyişəni 41-dən kiçik və ya bərabər olduğu müddətcə dövr edir
        while (x <= xn)
        {
            // Düsturu tam sadə şəkildə qururuq
            // Math.Cos(x) kosinus, Math.Tan(t) isə tangens funksiyasıdır
            double zx = Math.Cos(x) + 2 * a * Math.Tan(t);

            // Öyrəndiyimiz rahat üsulla ekrana çıxarırıq
            Console.WriteLine($"x = {x}  -->  z(x) = {zx}");

            // x-in qiymətini hər addımda 5 vahid artırırıq
            x += dx;
        }
    }
}
#sual4
using System;

class Program
{
    static void Main()
    {
        // Şəkildə verilən ilkin qiymətləri bəsit dəyişənlər olaraq təyin edirik
        double x = 1.0;          // x0 = 1
        double xn = 3.0;         // xn = 3
        double dx = 0.43;        // Delta x = 0.43

        Console.WriteLine("x qiymeti -- u(x) qiymeti");
        Console.WriteLine("-----------------------");

        // x dəyişəni 3-dən kiçik və ya bərabər olduğu müddətcə dövr davam edir
        while (x <= xn)
        {
            // Düsturu tam sadə şəkildə qururuq
            // Math.Exp(x) -> e üstü x deməkdir
            // Math.Log10(x) -> lg x (10luq loqarifm) deməkdir
            double ux = Math.Exp(x) - 5.6 * Math.Log10(x);

            // Öyrəndiyimiz rahat üsulla ekrana çıxarırıq
            Console.WriteLine($"x = {x}  -->  u(x) = {ux}");

            // x-in qiymətini hər addımda 0.43 artırırıq
            x += dx;
        }
    }
}
#sual5
using System;

class Program
{
    static void Main()
    {
        // Şəkildəki ikinci məsələnin ilkin qiymətlərini təyin edirik
        double x = 1.0;          // x0 = 1
        double xn = 7.0;         // xn = 7
        double dx = 0.85;        // Delta x = 0.85
        double a = 21.0;         // a = 21

        Console.WriteLine("x qiymeti -- w(x) qiymeti");
        Console.WriteLine("-----------------------");

        // x dəyişəni 7-dən kiçik və ya bərabər olduğu müddətcə dövr davam edir
        while (x <= xn)
        {
            // Düsturu tam sadə şəkildə qururuq
            // a / x birbaşa bölmədir, Math.Acos(x) is' arkkosinusdur
            double wx = (a / x) - Math.Acos(x);

            // Öyrəndiyimiz rahat üsulla ekrana çıxarırıq
            Console.WriteLine($"x = {x}  -->  w(x) = {wx}");

            // x-in qiymətini hər addımda 0.85 artırırıq
            x += dx;
        }
    }
}
