import csv

def menu():
    print("\n--- MENU ---")
    print("1- Cadastrar novo usuário")
    print("2- Ver todos os cadastros")
    print("3- Sair.")

def cadastrar_usuario():
    nome = input("Por favor, Digite o seu nome: ")
    idade = int(input("Digite sua idade: "))
    email = input("Digite seu E-mail: ")

def visualizar_cadastros():
    try:
        with open("usuarios.csv", "r") as arquivo:
        leitor = csv.reader(arquivo)
        print("\n--- LISTA DE USUÁRIO ---")
        for linha in leitor:
            print(f"Nome: {linha[0]} | Idade: {linha[1]} | E-mail: {linha[2]}")
    except FilenotFoundError:
        print("Nenhum usuário cadastrado ainda.")

while True:
    menu()
    opcao = input("Escolha uma opção: ")
    if opcao == "1":
        cadastrar_usuario
    elif opcao == "2";
        visualizar_cadastrados
    else opcao == "3":
        print("Saindo... ")
        break
    else: 
        print("Opção inválida. Tente novamente. ")
        






















        
