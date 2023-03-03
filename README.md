# TesteEstagio
using System;

class Program {
    static void Main() {
        Console.Write("Insira um número: ");
        int n = int.Parse(Console.ReadLine());

        int a = 0, b = 1, c = 0;
        bool pertence = false;

        Console.Write("A sequência de fibonacci é: ");
        while (c <= n) {
            if (c == n) {
                pertence = true;
            }
            Console.Write(c + " ");
            a = b;
            b = c;
            c = a + b;
        }
        if (pertence) {
            Console.WriteLine("O número " + n + " pertence a sequência de Fibonacci.");
        } else {
            Console.WriteLine("O número " + n + " não pertence a sequência de Fibonacci.");
        }
    }
}
