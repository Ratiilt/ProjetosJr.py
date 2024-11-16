# ProjetosJr.py
Projetos de aprendizagem em Python.


import random


numero_secreto = random.randint(1, 100)
i = True
tentativa = 0
limite_tentativa = 10

while i:
    
    numero_escolhido = int(input("Escolha seu numero!!! "))
    tentativa += 1
    print(f"tentativa = {tentativa}")
    
    
    if numero_escolhido == numero_secreto:
        print(f"Você acertou, o numero era {numero_secreto}")
        i = False
    
    elif tentativa == limite_tentativa:
        print("Você nao conseguiu completar o jogo ")
        i = False

    elif numero_escolhido > numero_secreto:
        print(f"O numero correto é menor que {numero_escolhido}")
    
    elif numero_escolhido < numero_secreto:
        print (f" O numero correto é maior que {numero_escolhido}")



