[Uploading # dET# dETECTOR De N primos
#Aqui ele está verificando
def is_prime(numero):
    if numero <= 1:
        return False  # Números menores ou iguais a 1 não são primos
    for i in range(2, int(numero ** 0.5) + 1):
        if numero % i == 0:
            return False  # Encontrou um divisor, não é primo
    return True  # Nenhum divisor encontrado, é primo

#Aqui é a pergunta em si
while True:
    try:
        # Solicita um número inteiro
        numero = int(input("Enter a number to check if it's prime: "))
        
        # Verifica se é primo
        if is_prime(numero):
            print(f"{numero} is a prime number!")
        else:
            print(f"{numero} is not a prime number.")
        
        # Pergunta ao usuário se deseja continuar
        repeat = input("Do you want to check another number? (yes/no): ").strip().lower()
        if repeat != "yes":
            print("Goodbye!")
            break  # Sai do loop se o usuário digitar algo diferente de 'yes'
    except ValueError:
        print("Invalid input. Please enter a valid number.")ECTOR De N primos.py…]()
