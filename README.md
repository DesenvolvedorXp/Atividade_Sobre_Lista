# Atividade_Sobre_Lista
verifica até 10 caracteres, conta-os e mostra os caracteres. Falta implementar quando for digitado números
lista = []

aux = 0

caracteres = input('Digite 10 Caracteres>>> ').upper()

lista_caracteres = [caracteres]#Aqui, a variavel 'caracteres' vai se transformar numa lista. para poder acessar seus elemntos

for c in range(0, len(caracteres)):#Aqui, a repetição vai ocorre de acordo com o número de letras.
    if not lista_caracteres[0][c] in 'AEIOU':# Aqui se as vogais 'AEIOU' forem detectada não vai ser contada. Só as que não forem
        aux += 1
        x = lista.append(lista_caracteres[0][c])# vai pegar a letra que nãé vogal e vai inserir no final da lista, na variavel' lista'

print('Números de consoantes: {}, consoantes: {}'.format(aux, lista))
