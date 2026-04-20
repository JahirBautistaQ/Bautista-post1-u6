# Bautista-post1-u6
Unidad 6: Antipatrones de Diseño Post-Contenido 1

## Estudiante
Jahir Bautista

## Repositorio
Bautista-post1-u6

## Antipatrón identificado

Se identificó el antipatrón **God Object**, donde la clase `GestorBiblioteca`
concentraba múltiples responsabilidades.

## Responsabilidades encontradas

1. Gestión del catálogo de libros (agregar, buscar, listar)
2. Gestión de socios (registrar, validar, buscar)
3. Gestión de préstamos (prestar, devolver)
4. Generación de reportes del sistema

## Principio aplicado

Se aplicó el **Principio de Responsabilidad Única (SRP)**.

## Refactorización realizada

Se dividió `GestorBiblioteca` en:

- `CatalogoLibros`
- `RegistroSocios`
- `ServicioPrestamos`
- `GeneradorReportes`

Y se agregaron clases de dominio:

- `Libro`
- `Socio`

## Compilación y ejecución

```bash
mvn compile
mvn exec:java

<img width="1136" height="667" alt="image" src="https://github.com/user-attachments/assets/8dc9667a-5b43-4e58-a43e-2e8fd5346ffc" /> 
