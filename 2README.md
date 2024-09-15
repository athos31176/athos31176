Nome: Athos Guilherme de França Pereira

Projeto: Calculadora de operações simples

funcionalidade: calcular soma, adição, subtração, divisão e multiplicação.

Neste projeto envolve um pouco de tudo que vi ate hoje em Phyton, muito praseroso e dou total atribuição aos professores de BIG DATA.

def add(x, y):
    return x + y


def subtract(x, y):
    return x - y


def multiply(x, y):
    return x * y


def divide(x, y):
    if y == 0:
        return "Erro! Divisão por zero."
    return x / y


def main():
    print("Selecione a operação:")
    print("1. Adição")
    print("2. Subtração")
    print("3. Multiplicação")
    print("4. Divisão")

    while True:
        choice = input("Digite sua escolha (1/2/3/4): ")

        if choice in ['1', '2', '3', '4']:
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))

            if choice == '1':
                print(f"{num1} + {num2} = {add(num1, num2)}")

            elif choice == '2':
                print(f"{num1} - {num2} = {subtract(num1, num2)}")

            elif choice == '3':
                print(f"{num1} * {num2} = {multiply(num1, num2)}")

            elif choice == '4':
                print(f"{num1} / {num2} = {divide(num1, num2)}")
        else:
            print("Opção inválida. Tente novamente.")

        next_calculation = input("Deseja fazer outra operação? (sim/não): ")
        if next_calculation.lower() != 'sim':
            break


if __name__ == "__main__":
    main()
<!---
athos31176/athos31176 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
