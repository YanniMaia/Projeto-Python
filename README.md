# Projeto-Python

def main():
    valores = []
    while True:
        entrada = int(input("Digite um número real (ou 'sair' para finalizar): ")

        if entrada.lower() == " sair ":
            break   

        try:
            numero = float(entrada)  
            valores.append(numero)   
        except  ValueError:
            print("Entrada inválida! Digite um número real.")

    quantidade = len(valores)
    soma = sum(valores)
    media = soma / quantidade if quantidade > 0 else 0
    maiores_que_20 = sum(1 for num in valores if num > 20)

    print("\nResultados:")
    print(f"Quantidade de valores digitados: {quantidade}")
    print(f"Soma dos valores: {soma:.2f}")
    print(f"Média aritmética: {media:.2f}")
    print(f"Quantidade de valores maiores que 20: {maiores_que_20}")
