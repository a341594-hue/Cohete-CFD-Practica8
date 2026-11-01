# Simulacion CFD de un cohete - Practica 8

Universidad Autonoma de Chihuahua
Laboratorio de Aerofluidos

OpenFOAM Foundation 12 / blueCFD-Core 2024

Geometria: Space Shuttle Rocket Model
Autora del modelo CAD: Pamela Soliz
Fuente: GrabCAD Community

Se incluyen once configuraciones de estudio:
- Comparacion de mallas.
- Refinamiento de superficie y base.
- Dominio ampliado.
- Velocidades de 10, 15, 20, 25 y 30 m/s.

El caso de 30 m/s corresponde a:
cohete_prueba_superficie

Las carpetas contienen las condiciones iniciales,
propiedades, geometria y diccionarios de configuracion.

Se excluyen los campos volumetricos de resultados
y las mallas polyMesh generadas para reducir el tamaño.

Los archivos forceCoeffs incluidos son registros
de resultados de las simulaciones originales.

Nota: el archivo cohete_mm.stl esta en milimetros.
Se debe utilizar la geometria en metros indicada
por los diccionarios correspondientes.

## Creditos de la geometria

Modelo: Space Shuttle Rocket Model
Autora original: Pamela Soliz
Fuente: GrabCAD Community
https://grabcad.com/library/space-shuttle-rocket-model-1

Geometria adaptada y preparada para una
simulacion CFD academica sin fines comerciales.

## Reproduccion

Software: OpenFOAM Foundation 12
Modelo de turbulencia: kOmegaSST
Solver: foamRun -solver incompressibleFluid

Etapas de preparacion:
1. blockMesh
2. surfaceFeatures
3. snappyHexMesh
4. checkMesh
5. Ejecucion del solver configurado

Los archivos de cada caso permiten revisar los
parametros especificos de malla y condiciones
de frontera. El caso de 30 m/s es
cohete_prueba_superficie.
