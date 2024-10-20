# Práctica de Modelado y SQL - Johanna Díaz

## Descripción

Este proyecto tiene como objetivo desarrollar un sistema para gestionar un videoclub, permitiendo registrar socios, películas y los préstamos de las mismas. El sistema incluye un modelo de datos normalizado y un script SQL para crear y poblar la base de datos.

## Requisitos Funcionales

Durante la discusión sobre el videoclub, se identificaron los siguientes requisitos:

1. **Registro de Socios**: 
   - Información básica: nombre, apellidos, fecha de nacimiento, teléfono y número de identificación (DNI, Pasaporte, etc.).
   - Asignación de un número de socio para la creación de carnets.
   - Registro de dirección de correspondencia (opcional): código postal, calle, número y piso.

2. **Registro de Películas**:
   - Información de cada película: título, género, director y sinopsis.
   - Posibilidad de tener múltiples copias de cada película.

3. **Gestión de Préstamos**:
   - Registro del socio al que se ha prestado cada copia, incluyendo las fechas de préstamo y devolución.
   - Identificación de películas disponibles para alquilar (no prestadas), mostrando el título y el número de copias disponibles.

## Entregables

Esta práctica se entrega en dos partes:
1. **Diagrama Entidad/Relación**: Crear un diagrama en formato draw.io que represente el modelo de datos.
2. **Script SQL**: Un script que muestre qué películas están disponibles para alquilar en este momento (no están prestadas), mostrando el título de la película y el número de copias disponibles.

# Proceso de Realización - Práctica de Modelado y SQL

## Introducción

Este documento describe el proceso seguido para desarrollar el ejercicio de modelado y SQL para un videoclub, a partir de los requisitos funcionales proporcionados.

## Paso 1: Análisis de Requisitos

Se revisaron los requisitos del ejercicio y se identificaron las entidades clave necesarias para el modelo de datos:

1. **Socios**: Almacenar información sobre los socios del videoclub.
2. **Películas**: Registrar las películas disponibles, incluyendo copias.
3. **Préstamos**: Gestionar los préstamos de películas a los socios.

## Paso 2: Diseño del Modelo de Datos

Se elaboró un Diagrama Entidad/Relación (ER) que representa las entidades y sus relaciones. En el diagrama se incluyeron:

- **socios**: Atributos como nombre, apellidos, fecha de nacimiento, teléfono y dni.
- **correspondencia**: Atributos como registro del socio, código postal, calle, piso, número.
- **peliculas**: Atributos como título, género, director y sinopsis.
- **prestado**: Registro del socio que alquila la película, fechas de préstamo y devolución.
- **copias**: Atributos como registro de la copia y de la película.

## Paso 3: Normalización

Se aplicó normalización para asegurar que las tablas estén correctamente estructuradas, evitando redundancias y asegurando la integridad de los datos.

## Paso 4: Creación del Script SQL

Se desarrolló un script SQL que realiza las siguientes acciones:

1. **Creación de Esquema y Tablas**: Definición de las tablas para socios, peliculas, prestado, copias y correspondencia.
2. **Carga de Datos**: Inserción de datos de prueba.
3. **Consultas**: Implementación de consultas para:
   - Mostrar las películas disponibles para alquilar.

## Paso 5: Pruebas y Validación

Se ejecutó el script SQL en la base de datos para verificar que:
- Todas las tablas se crearan correctamente.
- Los datos se cargaran sin errores.
- Las consultas devolvieran resultados esperados.

## Conclusión

Al finalizar estos pasos, se logró completar el ejercicio de forma satisfactoria, cumpliendo con los requisitos y asegurando la funcionalidad del sistema de gestión del videoclub.


