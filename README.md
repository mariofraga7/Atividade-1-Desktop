# Atividade-1-Desktopusing System;

class Program
{
    static void Main()
    {
        // 1. Verificar maioridade
        Console.Write("Digite sua idade: ");
        int idade = int.Parse(Console.ReadLine());
        if (idade >= 18)
            Console.WriteLine("Você é maior de idade.");
        else
            Console.WriteLine("Você é menor de idade.");

        Console.WriteLine();

        // 2. Calcular média de 3 notas
        Console.Write("Digite a primeira nota: ");
        double nota1 = double.Parse(Console.ReadLine());
        Console.Write("Digite a segunda nota: ");
        double nota2 = double.Parse(Console.ReadLine());
        Console.Write("Digite a terceira nota: ");
        double nota3 = double.Parse(Console.ReadLine());
        double media = (nota1 + nota2 + nota3) / 3;
        if (media >= 7)
            Console.WriteLine("Aprovado.");
        else
            Console.WriteLine("Reprovado.");

        Console.WriteLine();

        // 3. Verificar se número é positivo ou negativo
        Console.Write("Digite um número: ");
        double numero = double.Parse(Console.ReadLine());
        if (numero >= 0)
            Console.WriteLine("Número positivo.");
        else
            Console.WriteLine("Número negativo.");

        Console.WriteLine();

        // 4. Verificar se número é par ou ímpar
        Console.Write("Digite um número inteiro: ");
        int inteiro = int.Parse(Console.ReadLine());
        if (inteiro % 2 == 0)
            Console.WriteLine("Número par.");
        else
            Console.WriteLine("Número ímpar.");

        Console.WriteLine();

        // 5. Calcular o dobro de um número
        Console.Write("Digite um número: ");
        double numDobro = double.Parse(Console.ReadLine());
        Console.WriteLine("O dobro é: " + (numDobro * 2));

        Console.WriteLine();

        // 6. Verificar se número é divisível por 3
        Console.Write("Digite um número: ");
        int numDiv3 = int.Parse(Console.ReadLine());
        if (numDiv3 % 3 == 0)
            Console.WriteLine("Divisível por 3.");
        else
            Console.WriteLine("Não é divisível por 3.");

        Console.WriteLine();

        // 7. Soma de 1 até N com for
        Console.Write("Digite um número inteiro positivo N: ");
        int N = int.Parse(Console.ReadLine());
        int soma = 0;
        for (int i = 1; i <= N; i++)
        {
            soma += i;
        }
        Console.WriteLine("A soma de 1 até " + N + " é: " + soma);

        Console.WriteLine();

        // 8. Ler 10 números e contar os pares com while
        int contador = 0;
        int pares = 0;
        while (contador < 10)
        {
            Console.Write("Digite um número inteiro: ");
            int valor = int.Parse(Console.ReadLine());
            if (valor % 2 == 0)
                pares++;
            contador++;
        }
        Console.WriteLine("Quantidade de números pares: " + pares);
    }
}
