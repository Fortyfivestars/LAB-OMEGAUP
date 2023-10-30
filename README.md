#PROBLEMA 1 
# Lee la cantidad de segundos que marca tu reloj y la cantidad de segundos que debería marcar
segundos_marcados = int(input())
segundos_correctos = int(input())

# Calcula la diferencia entre los segundos marcados y los segundos correctos
diferencia = segundos_correctos - segundos_marcados

# Determina si debes adelantar o atrasar el reloj y en qué cantidad de segundos
if diferencia > 0:
    if diferencia == 1:
        print("ADELANTAR 1 SEGUNDO")
    else:
        print(f"ADELANTAR {diferencia} SEGUNDOS")
elif diferencia < 0:
    if abs(diferencia) == 1:
        print("ATRASAR 1 SEGUNDO")
    else:
        print(f"ATRASAR {abs(diferencia)} SEGUNDOS")
else:
    print("HORA CORRECTA")
