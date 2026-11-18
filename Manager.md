import random

print("Parabens, voce virou um jogador!")
print("Escolha um clube")

# ESCOLHA DO CLUBE
while True:
    print("\n1 - Flamengo")
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

# ESCOLHA DA POSICAO
print("\nAgora escolha a sua posicao")

while True:
    print("\n1 - Zagueiro")
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

# PRIMEIRO JOGO
print("\nVoce ira para o seu primeiro jogo!")
print("Minuto 54 - O jogo esta empatado, voce tem a chance de fazer o gol da vitoria.")

chute = int(input("Digite 1 para chutar ou 2 para passar a bola: "))

if chute == 1:
    print("Voce chutou e fez o gol da vitoria!!")

elif chute == 2:
    print("Voce passou a bola e o seu companheiro errou o chute.")
    print("O jogo terminou empatado.")
    print("O tecnico reclamou com voce e mandou voce melhorar o seu desempenho.")
    print("Voce foi para o banco de reservas e nao jogou mais na temporada.")

else:
    print("Escolha invalida.")

# DIA DE TREINO
print("\nDia de treino")

treino = int(input("Digite 1 para treinar ou 2 para descansar: "))

if treino == 1:
    print("Voce treinou e melhorou o seu desempenho.")
    print("Voce foi titular na proxima partida.")

else:
    print("Voce descansou e nao melhorou o seu desempenho.")
    print("Voce foi para o banco de reservas na proxima partida.")

# PROPOSTA EUROPEIA
print("\nSeu destaque na temporada chamou a atencao de um clube europeu!")
print("Voce recebeu uma proposta para jogar na Europa.")

proposta = int(input("Digite 1 para aceitar a proposta ou 2 para recusar: "))

if proposta == 1:
    print("Voce aceitou a proposta e foi jogar na Europa.")
    print("Voce se destacou e se tornou um dos melhores jogadores do mundo.")

else:
    print("Voce recusou a proposta e continuou jogando no Brasil.")
    print("Voce se destacou e se tornou um dos melhores jogadores do mundo.")

# COPA DO MUNDO
print("\nPerto da sua aposentadoria, sua selecao te convocou para jogar a Copa do Mundo.")
print("Voce foi titular e ajudou sua selecao a chegar na final.")

print("\nO jogo foi para os penaltis!")
print("Voce foi o ultimo a bater e precisava fazer o gol da vitoria.")

# COBRANCA DO PENALTI
print("\nEscolha o canto que voce deseja chutar:")
print("1 - Canto esquerdo")
print("2 - Canto direito")
print("3 - Meio do gol")

cobranca = int(input("Digite o numero do canto que voce deseja chutar: "))

goleiro = random.randint(1, 3)

if cobranca == goleiro:
    print("\nO goleiro defendeu!")
    print("Voce perdeu a final e sua selecao ficou com o vice-campeonato.")

elif cobranca in [1, 2, 3]:
    print("\nGOOOOOL!!")
    print("Voce fez o gol da vitoria!")
    print("Sua selecao se tornou campea do mundo.")
    print("Voce se tornou um heroi nacional e foi eleito o melhor jogador da Copa do Mundo.")

else:
    print("Escolha invalida.")
