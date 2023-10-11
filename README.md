- 👋 Hi, I’m @todxan04
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
todxan04/todxan04 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
def crear_matriz(filas, columnas):
    matriz = []
    for i in range(filas):
        fila = []
        for j in range(columnas):
            valor = int(input(f"Ingrese el valor para la posición ({i+1},{j+1}): "))
            fila.append(valor)
        matriz.append(fila)
    return matriz

def mostrar_matriz(matriz):
    for fila in matriz:
        print(fila)

filas = int(input("Ingrese la cantidad de filas: "))
columnas = int(input("Ingrese la cantidad de columnas: "))

matriz = crear_matriz(filas, columnas)

print("\nMatriz resultante:")
mostrar_matriz(matriz)
