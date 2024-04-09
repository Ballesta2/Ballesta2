lista = ["router","pc","hub"]


lista[2] = "bridge" #modificando
lista.append("camara") #agregando
lista.insert(1, "cloud")
lista.remove("camara")

para automatizar
es 
nuevodispositivo = input("que dispositivo quieres agregar:  ")
lista.append(nuevodispositivo)



discionario

grupo_personas = {
    "persona1": {
        "nombre": "Ana",
        "edad": 25,
        "ciudad": "Madrid"
    },
    "persona2": {
        "nombre": "Pedro",
        "edad": 30,
        "ciudad": "Barcelona"
    },
    "persona3": {
        "nombre": "Mar铆a",
        "edad": 28,
        "ciudad": "Sevilla"
    }
}

# Acceder a la informaci贸n de la persona2
print(grupo_personas["persona2"])  
# Output: {'nombre': 'Pedro', 'edad': 30, 'ciudad': 'Barcelona'}

# Acceder al nombre de la persona3
print(grupo_personas["persona3"]["nombre"])  
# Output: Mar铆a

# Acceder a la edad de la persona1
print(grupo_personas["persona1"]["edad"])  
# Output: 25


-------------------------------
def menu():
    print("Bienvenido a nuestro men煤.")
    print("Opci贸n 1: Variables y Operadores L贸gicos")
    print("Opci贸n 2: Uso de Listas, Tuplas y Diccionarios")
    print("Opci贸n 3: Uso de if y else")
    print("Opci贸n 4: Bucles ")  
    print("Opci贸n 5: Salir del men煤")

def mostrar_volver():
    print("Opci贸n 6: Volver al men煤 principal")

def opcion_1():
    ancho = int(input("Ancho de banda en mbps: "))
    latencia = int(input("Latencia en segundos:  "))
    print("Informaci贸n ingresada:", ancho , latencia)
    if ancho >= 1000 and latencia <= 1:
        print("La conexi贸n es 贸ptima")
    else:
        print("La conexi贸n no es 贸ptima")

def opcion_2():
    lista = ["R1","R2","R3","R4","R5"]
    print(lista)
    R1 = ("R1","IP:192.168.1.1","ID=1.1.1.1")
    R2 = ("R2","IP:192.168.2.2","ID=2.2.2.2")
    R3 = ("R3","IP:192.168.3.3","ID=3.3.3.3")
    R4 = ("R4","IP:192.168.4.4.","ID=4.4.4.4")
    for x in R1,R2,R3,R4:
        print(x)

while True:
    menu()
    mostrar_volver()
    opcion = input("Elige una opci贸n: ")

    if opcion == "1":
       opcion_1() 
    elif opcion == "2":
        opcion_2()
    elif opcion == "5":
        print("Saliendo del men煤")
        break
    elif opcion == "6":
        continue
    else:
        print("Opcion no valida. Por favor, elige una opci贸n v谩lida.")
