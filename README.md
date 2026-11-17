# football-career-simulator

import random

print("Parabens, voce virou um jogador!")

print("Escolha um clube")

while True:
    print("1 - Flamengo")
    print("2 - Palmeiras")
    print("3 - Corinthians")
    print("4 - Sao Paulo")

    escolha = int(input("Digite o numero do clube que voce deseja escolher: "))

    if escolha == 1:
        print("Voce escolheu o Flamengo")
        break
    elif escolha == 2:
        print("Voce escolheu o Palmeiras")
        break
    elif escolha == 3:
        print("Voce escolheu o Corinthians")
        break
    elif escolha == 4:
        print("Voce escolheu o Sao Paulo")
        break
    else:
        print("Escolha invalida, tente novamente.")

print("Agora escolha a sua posicao")

while True:
    print("1 - Zagueiro")
    print("2 - Lateral")
    print("3 - Meio-campista")
    print("4 - Atacante")

    posicao = int(input("Digite o numero da posicao que voce deseja jogar: "))

    if posicao == 1:
        print("Voce escolheu ser zagueiro")
        break
    elif posicao == 2:
        print("Voce escolheu ser lateral")
        break
    elif posicao == 3:
        print("Voce escolheu ser meio-campista")
        break
    elif posicao == 4:
        print("Voce escolheu ser atacante")
        break
    else:
        print("Escolha invalida, tente novamente.")

print("Voce ira para o seu primeiro jogo")

print("Minuto 54 - O jogo esta empatado, voce tem a chance de fazer o gol da vitoria")

chute = int(input("Digite 1 para chutar ou 2 para passar a bola: "))

if chute == 1:
    print("Voce chutou e fez o gol da vitoria!!")
elif chute == 2:
    print("Voce passou a bola e o seu companheiro errou o chute, o jogo terminou empatado")
    print("O tecnico reclamou com voce e mandou voce melhorar o seu desempenho. Voce foi para o banco de reservas e nao jogou mais na temporada")
else:
    print("Escolha invalida.")

print("Dia de treino")

treino = int(input("Digite 1 para treinar ou 2 para descansar: "))

if treino == 1:
    print("Voce treinou e melhorou o seu desempenho, voce foi titular na proxima partida")
else:
    print("Voce descansou e nao melhorou o seu desempenho, voce foi para o banco de reservas na proxima partida")

print("Seu destaque na temporada chamou a atencao de um clube europeu, voce recebeu uma proposta para jogar na Europa")

proposta = int(input("Digite 1 para aceitar a proposta ou 2 para recusar: "))

if proposta == 1:
    print("Voce aceitou a proposta e foi jogar na Europa, voce se destacou e se tornou um dos melhores jogadores do mundo")
else:
    print("Voce recusou a proposta e continuou jogando no Brasil, voce se destacou e se tornou um dos melhores jogadores do mundo")

print("Perto da sua aposentadoria, sua selecao te convocou para jogar a copa do mundo, voce foi titular e ajudou a sua selecao a chegar na final.")

print("O jogo foi para os penaltis, voce foi o ultimo a bater e tinha que fazer o gol da vitoria para a sua selecao ser campea do mundo")

print("\nEscolha o canto que voce deseja chutar:")
print("1 - Canto esquerdo")
print("2 - Canto direito")
print("3 - Meio do gol")

cobranca = int(input("Digite o numero do canto que voce deseja chutar: "))

goleiro = random.randint(1, 3)

if cobranca == goleiro:
    print("\nO goleiro defendeu")
    print("Voce perdeu a final e a sua selecao ficou com o vice-campeonato")
elif cobranca in [1, 2, 3]:
    print("\nGOOOOOL!!")
    print("Voce fez o gol da vitoria e a sua selecao se tornou campea do mundo, voce se tornou um heroi nacional e foi eleito o melhor jogador da copa do mundo")
else:
    print("Escolha invalida.")
