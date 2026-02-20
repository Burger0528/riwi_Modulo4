# Academic Management Database

**Project Name:** gestion_academica_universidad  
**Database Type:** MySQL  

---

## Project Description

This project consists of designing and implementing a relational academic database system that manages:

- Students  
- Teachers  
- Courses  
- Enrollments  

The system stores academic information and allows performance analysis using SQL features such as DDL, DML, DQL, aggregate functions, subqueries, and views.

---

## Database Structure

The database contains four main tables:

### 1. Students (`estudiantes`)

Stores student personal and academic information.

**Fields:**
- `id_estudiante` (Primary Key, Auto Increment)
- `nombre_completo`
- `correo_electronico` (UNIQUE)
- `genero`
- `identificacion` (UNIQUE)
- `carrera`
- `fecha_nacimiento`
- `fecha_ingreso`

---

### 2. Teachers (`docentes`)

Stores teacher information.

**Fields:**
- `id_docente` (Primary Key, Auto Increment)
- `nombre_completo`
- `correo_institucional` (UNIQUE)
- `departamento_academico`
- `anios_experiencia`

**Relationship:**
- One teacher can teach multiple courses (1:N).

---

### 3. Courses (`cursos`)

Stores academic courses.

**Fields:**
- `id_curso` (Primary Key, Auto Increment)
- `nombre`
- `codigo` (UNIQUE)
- `creditos`
- `semestre`
- `id_docente` (Foreign Key)

---

### 4. Enrollments (`inscripciones`)

Bridge table between students and courses.

**Fields:**
- `id_inscripcion` (Primary Key, Auto Increment)
- `id_estudiante` (Foreign Key)
- `id_curso` (Foreign Key)
- `fecha_inscripcion`
- `calificacion_final`

**Relationship:**
- Many-to-Many between students and courses, resolved through the enrollments table.

---

## SQL Features Implemented

### DDL (Data Definition Language)
- CREATE DATABASE
- CREATE TABLE
- ALTER TABLE
- DROP DATABASE

### DML (Data Manipulation Language)
- INSERT
- DELETE

### DQL (Data Query Language)
- SELECT
- JOIN
- GROUP BY
- HAVING
- Subqueries

### Aggregate Functions
- AVG()
- COUNT()
- SUM()
- MAX()
- MIN()
- ROUND()

### Constraints
- PRIMARY KEY
- FOREIGN KEY
- NOT NULL
- UNIQUE
- CHECK
- ON DELETE (CASCADE / SET NULL)

---

## Analytical Queries Included

- Students enrolled in more than one course  
- Courses with more than two students  
- Average grade per course  
- Students above the overall average  
- Academic performance indicators  

---

## View Created

### vista_historial_academico

This view displays:

- Student name  
- Course name  
- Teacher name  
- Semester  
- Final grade  

The view simplifies academic performance analysis and avoids repeating complex JOIN operations.

---

## Project Description. 
 ANDRES HURTADO

