-- Crear la base de datos
CREATE DATABASE concesionaria;

-- Crear tablas
CREATE TABLE AUTOS (
	id_patente varchar(10) NOT NULL,
    marca varchar(40) NOT NULL,
    Año int,
    precio decimal(15, 2),
    color varchar(20),
    combustible varchar(20),
    carroceria varchar (20)
);

CREATE TABLE AGENCIA (
	id_agencia int NOT NULL,
    nombre varchar(20) NOT NULL,
    ubicacion varchar(20),
    patente varchar (10),
    legajo int
);

CREATE TABLE EMPLEADOS (
	id_legajo int NOT NULL,
    nombre varchar (20) NOT NULL,
    apellido varchar (20) NOT NULL,
    correo varchar(50),
    Telefono int NOT NULL
);

CREATE TABLE VENTAS (
	id_ventas int NOT NULL,
    dni int NOT NULL,
    monto decimal (10, 2),
    patente varchar(10),
    fecha_venta date,
    legajo int
    
);

CREATE TABLE CLIENTES (
	id_dni int NOT NULL,
    nombre varchar (20) NOT NULL,
    apellido varchar (20) NOT NULL,
    telefono int,
    correo varchar (40) NOT NULL,
    direccion varchar (40) NOT NULL
);
    
