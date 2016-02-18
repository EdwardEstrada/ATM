# Simulacion de Cajero Automatico
# Creado por Edward Estrada - Lucia Moreira - Jefferson Baque
# Python 3.5.1 - 18-02-2016

import sys

print("Bienvenido a BANRED")
print("Seleccione una opción: ")
print("1 - Retiro de Efectivo")
print("2 - Consulta de Saldos")
print("3 - Cancelar")
     
#Entrada interactiva
     
opcion = input("> ")
     

if opcion == "1":
  print("Favor elija la cantidad a retirar") 
  print("Presione a = 10, b = 20, c = 40, d = 50, e = 60, f = 80, g = otro valor")
       
elif opcion == "2":
  print("Elija el tipo de cuenta")
  print("1 - Cuenta Corriente")
  print("2 - Cuenta Ahorro")
  
  tipo_cuenta = input("> ")

  print("Su saldo es de 2000 dólares")
  sys.exit(3)

elif opcion == "3":
  print("Gracias por su preferencia")
  sys.exit(3)

#Definicion de opciones
     
retiro = input("> ")
a = 10
b = 20
c = 30
d = 50
e = 60
f = 80
monto = 200

if retiro =="g":
  print("Ingrese cantidad a retirar")
  monto = input()
  monto = int(monto)

if monto > 200:
  print("Monto no permitido. Transacciòn Finalizada")
  sys.exit(3)
  
if retiro == "a" or "b" or "c" or "d" or "e" or "f" or "g":
 print("Retire su dinero, gracias por utilizar nuestro servicio.")
     
elif retiro != "a" or "b" or "c" or "d" or "e" or "f" or "g":
  print("Opcion no valida, intente de nuevo.")
