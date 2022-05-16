# lista
evaluacion

#hacer una lista y sumar los impares

lista = (3,5,2,9,7,8,12,15,18)

def sumar_impares(lista):
    if len (lista) ==0:
        return 0
    elif lista[0] % 2 ==0:
        return lista[0] + sumar_impares(lista[1 :])
    else:
        return sumar_impares(lista[1 :])
print (sumar_impares(lista))
