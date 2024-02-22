lista = []

while True:
    nome = input("Digite o nome do aluno: ")
    nota1 = float(input("Digite a 1° nota: "))
    nota2 = float(input("Digite a 2° nota: "))
    media = (nota1 + nota2)/2
    lista_aluno = [nome, nota1, nota2,  media]
    lista.append(lista_aluno)
    escolha = input("Quer continuar? s/n: ")
    if escolha == 'n':
        break

print("-----------------------------------------------------------------------")
print("|     Aluno     |      Nota 1     |     Nota 2      |      Média      |")
print("-----------------------------------------------------------------------")
for i in range (len(lista)):
    for j in range (len(lista_aluno)):
        print("{: ^15}".format(lista[i][j]), end=" | ")
    print("\n-----------------------------------------------------------------------")
# dados_cliente = {
#     "Nome": "Renan",
#     "Endereco": "Rua Cruzeiro",
#     "Telefone": "92324923"
# }

# print(dados_cliente)

# dados_cliente.pop('Telefone', None) #Ou del dados_cliente['Telefone']

# print(dados_cliente)

# cliente1 = {
#     "Nome" : "Marcelo",
#     "Sobrenome": "Grilo",
#     "Idade": "30"
# }
# cliente2 = {
#     "Nome" : "Pedro",
#     "Sobrenome": "Lucas",
#     "Idade": "24"
# }

# clientes = [cliente1, cliente2]
# #print(clientes[1][0])<-- ERRO
# print(clientes[1]["Nome"]) #<-- Certo