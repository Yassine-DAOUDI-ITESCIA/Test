# Test
mot1 = input('Veuillez taper votre 1er mot: ')
mot2 = input('Veuillez taper votre 2nd mot: ')
distanceH = 0
b = 0
def distance_hamming(mot1, mot2):
    global b
    global distanceH
    for i in mot1:
        if len(mot1) != len(mot2):
            print('les deux mots doivent avoir le même nombre de caractère')
            break
        elif i != mot2[b]:
            distanceH+=1
        b = b + 1

distance_hamming(mot1, mot2)
print("la distance de haming entre ces deux mots est de :", distanceH)
