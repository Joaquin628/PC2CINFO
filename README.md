# Ejercicio 2
import pandas as pd

df1 = pd.read_csv("ventas.txt", skiprows=1, nrows=3)
print(df1)

#Ejercicio 3
df2 = pd.read_csv("empleados.txt", skiprows=1, nrows=4, delim_whitespace=True)
print(df2)

#Ejercicio 4
pregunta3 = pd.read_csv("clientes.csv", skiprows=1, nrows=2)
print(pregunta3)

#Ejercicio 5
ejercicio4 = pd.read_csv("productos.csv", nrows=3)
print(ejercicio4)

#Ejercicio 6
df = pd.read_excel("C:/Users/Lenovo/OneDrive/Desktop/Clases python/Módulo 2/Proyecto calificado_ Pandas/ReportePersonal")

#Ejercicio 7
df = pd.read_excel("C:/Users/Lenovo/OneDrive/Desktop/Clases python/Módulo 2/Proyecto calificado_ Pandas/ReportePersonal", skiprows=4)
df = df.drop([0, 1])

#Ejercicio 9
df = df[[
    "N° HCL",
    "APTITUD",
    "APELLIDOS Y NOMBRES",
    "F. NAC.",
    "EDAD",
    "LUGAR DE NACIMIENTO",
    "PESO",
    "CARGO",
    "TIPO DE EMO"
]]
print(df.head(80))
print(df["EDAD"].describe())
