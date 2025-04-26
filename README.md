# repositório




import random

print("bemvindo ao jogo  de adivinnhaçao")
print("estou pensando em um numero entre 1 e 100")

numero_secreto = random.randint(1, 100)

tentativa = int(input("qual numero voce acha que e ?"))

#verifica se acertou

if tentativa == numero_secreto:
    print("parabens, voce acertou o numero")
else:
    print("voce errou, tente novamente")
    #verifica se o numero e maior ou menor 
    if tentativa < numero_secreto:
        print("o numero e maior")
    else:
        print("o numero e menor")
        #perguntar se quer continuar jogando
continuar = (input("voce quer continuar jogando? (s/n") )

if continuar == "s":
    print("ok,vamos jogar novamente")
    #reniciar o jogo
    numero_secreto = random.randint(1,100)
    tentativa = int(input("qual numero voce acha que e ?"))
    
    #verifica se acertou
    if tentativa == numero_secreto:
        print("parabens,voce acertou o numero")
    else:
        print("voce errou, tente novamente")