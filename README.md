# CRUD_MVC_5

Proyecto en ASP .NET MVC

=================================================.

Este es un pequeño proyecto que realiza un Alta, Ver, Actualizar y Eliminar registros con SQL Server y ASP .NET MVC. 

Se utilizo una Base de datos de prueba y una tabla de empleado. Se Agregan los Script para la creación de la base de datos y la tabla.

-- Script 1
-------------------------------------------
-- Crea base de datos

CREATE TABLE [db_prueba]
-------------------------------------------

-- Script 2
-------------------------------------------
USE db_prueba

GO

-- Crea tabla de Empleado

CREATE TABLE dbo.Empleado
(
	 Pk_Empleado INT IDENTITY(1,1) PRIMARY KEY
	,Nombre NVARCHAR(50)
	,Ape_Paterno NVARCHAR(50)
	,APe_Materno NVARCHAR(50)
	,Edad INT
	,Telefono INT
)
--------------------------------------------

-- Script 3
USE db_prueba
GO
--------------------------------
-- Se ingrega un registro para validar el correcto funcionamiento de nuestra pantalla

INSERT INTO dbo.Empleado (Nombre, Ape_Paterno, APe_Materno, Edad, Telefono ) VALUES ('Fernando', 'Hernández', 'López', 20, 55123455)
