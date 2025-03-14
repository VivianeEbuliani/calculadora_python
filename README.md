def soma(a,b):
    return a + b
def subtracao (a,b):
    return a - b
def multiplicacao (a,b):
    return a * b
def divisao (a,b):
    if b != 0:
        return a/b
    else:
        return "Não é possivel dividir por 0"
    
print ("Escolha uma operação:")
print("1. Soma")
print("2. Subtração")
print("3. Multiplicação")
print("4. Divisão")

operacao = input("Digite o numero da operação: ")

num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

if operacao == "1":
    print(f"{num1} + {num2} = {soma(num1, num2)}")
elif operacao == '2':
    print(f"{num1} - {num2} = {subtracao(num1,num2)}")
elif operacao == "3":
    print(f"{num1} * {num2} = {multiplicacao(num1,num2)}")
elif operacao == "4":
    print(f"{num1} / {num2} = {divisao(num1,num2)}")
else: 
    print("Operação inválida")
