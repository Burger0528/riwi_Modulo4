# Hospital Vida Sana Database Design

This project contains the database design for Hospital Vida Sana

It includes:

- Entity-Relationship Diagram (DER)
- Relational Model

The design manages:

- Patients
- Doctors
- Appointments
- Diagnoses

---

## Files

### DER.md
This file shows the conceptual model.
It includes:
- Entities
- Attributes
- Primary Keys
- Relationships

This model does not include data types.

---

### ModeloRelacional.md
This file shows the relational model.
It includes:
- Tables
- Data types
- Primary Keys
- Foreign Keys

This model is ready to be implemented in a database system.

---

## Relationships

- One patient can have many appointments.
- One doctor can have many appointments.
- One appointment has one diagnosis.

---

## Normalization

The database is normalized up to Third Normal Form (3NF).

- No repeated data.
- No partial dependencies.
- No transitive dependencies.

---

## Author

Andres hurtado 