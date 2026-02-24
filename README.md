# Csharp - Aulas

## Aula 24/02
### Par ou ímpar
```
// Descobrir se é ímpar ou par o número que o usuário digitar 
Console.WriteLine("BEM VINDO AO ÍMPAR PAR!!!");

Console.WriteLine("Digite um número inteiro para verificar se ele é par ou ímpar: "); // Pergunta
string entradaUsuario = Console.ReadLine(); // Lendo a linha

int numero; // Criando a variável de numero = inteiro

if (int.TryParse(entradaUsuario, out numero)) // 
{
    string resultado = (numero % 2 == 0) ? "PAR" : "ÍMPAR";
    Console.WriteLine(resultado);
}
else
{
    Console.WriteLine("Entrada inválida");
}
```
### Impressão da Tabuada
```
// Programa que imprime a tabuada
Console.WriteLine("Digite um número para ver a tabuada: "); // Imprime início
int numero = Convert.ToInt32(Console.ReadLine()); // Define o numero como int e converte para texto

Console.WriteLine($"Tabuada do {numero}"); // Texto e puxa o número

for (int i = 1; i <= 10; i++) // Repetição até 10
{
    Console.WriteLine($"{numero} x {i} = {numero * i}"); // Multiplica e imprime a tabuada
}

```

### Soma dos números em um array
```
// Programa que soma os itens de uma lista
int[] numeros = { 10, 20, 30, 40, 50, 60 }; // Lista de números
int soma = 0; // Soma começa com 0

foreach (int i in numeros) // Para cada item da lista na lista números
    soma += i; // A soma vai ser igual ao item += outro item

Console.WriteLine($"A soma dos números é: {soma}"); // Imprime a resposta

```
### Número válido
```
int numero; // Número como inteiro
do
{
    Console.WriteLine("Digite um número positivo");
    numero = Convert.ToInt32(Console.ReadLine());

    if (numero < 0)
    {
        Console.WriteLine("Número inválido");
    }

} while (numero < 0);

Console.WriteLine($"Número válido inserido: {numero}");
```
### Contagem Regressiva
```
Console.WriteLine(contador);

while (contador > 0)
{
    Console.WriteLine(contador);
    contador--;
}
```
### Tabuada do 1 ao 5 (loop aninhado)
```
Console.WriteLine("Tabuada do 1 ao 5:");

for (int i = 1; i <= 5; i ++)
{
    Console.WriteLine($"\nTabuada do {i}");

    for (int j = 1; j <= 10; j++)
        Console.WriteLine($"{i} x {j} = {i * j}");
};
```

