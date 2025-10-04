🚗 Enunciado — Sistema de Alquiler de Vehículos (Versión con Menú)

Una empresa de alquiler de vehículos desea un sistema para gestionar su flota y las operaciones de alquiler y devolución.

Requisitos:
1️⃣ Clase abstracta Vehiculo

Todos los vehículos comparten los siguientes atributos:

marca

modelo

precioPorDia

disponible (booleano)

Y el siguiente método abstracto:

calcularCosto(int dias) → devuelve el costo del alquiler según el tipo de vehículo.

2️⃣ Clases hijas:

Auto: el costo se calcula con un impuesto del 10% sobre el total (precioPorDia * días * 1.1).

Moto: el costo se calcula con un descuento del 5% (precioPorDia * días * 0.95).

3️⃣ Clase ServicioAlquiler

Esta clase mantiene una lista de vehículos (autos y motos).
Debe permitir:

Listar vehículos disponibles.

Alquilar un vehículo (si está disponible → marcar como no disponible).

Devolver un vehículo (marcarlo como disponible).

Calcular el costo del alquiler según los días y el tipo de vehículo.

4️⃣ Clase Main (menú principal)

Muestra opciones como:

----- MENÚ PRINCIPAL -----
1. Listar vehículos disponibles
2. Alquilar un vehículo
3. Devolver un vehículo
4. Salir
--------------------------
Ingrese una opción:


El programa deberá permitir:

Mostrar los vehículos que estén disponibles.

Solicitar al usuario la placa o modelo del vehículo para alquilarlo o devolverlo.

Mostrar el costo del alquiler al finalizar.
