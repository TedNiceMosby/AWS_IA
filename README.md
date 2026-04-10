# 🚀 AWS Python Projects Collection

Colección de scripts en Python para automatizar tareas comunes en AWS usando **boto3**.
Ideal para practicar, aprender y construir herramientas útiles en la nube.

---

## 📌 Tabla de Contenidos

1. [Automatizador de subida a S3](#1-automatizador-de-subida-de-archivos-a-amazon-s3)
2. [Backups automáticos a S3](#2-sistema-automático-de-backups-a-s3)
3. [Monitor de instancias EC2](#3-monitor-de-instancias-ec2)
4. [Limpieza automática de S3](#4-script-para-limpiar-buckets-s3-automáticamente)
5. [Alertas con CloudWatch](#5-sistema-simple-de-alertas-con-cloudwatch)
6. [Generador de usuarios IAM](#6-generador-automático-de-usuarios-iam)
7. [Inventario de recursos AWS](#7-inventario-de-recursos-aws)

---

## 🛠️ Requisitos

* Python 3.8+
* boto3
* AWS CLI configurado (`aws configure`)

Instalación de dependencias:

```bash
pip install boto3
```

---

## 1. Automatizador de subida de archivos a Amazon S3

### 🎯 Objetivo

Subir, listar y descargar archivos desde un bucket S3.

### ⚙️ Funcionalidades

* Subir un archivo
* Listar archivos
* Descargar un archivo

---

## 2. Sistema automático de backups a S3

### 🎯 Objetivo

Realizar backups automáticos de una carpeta local hacia S3.

### ⚙️ Funcionalidades

* Escanear una carpeta
* Subir todos los archivos
* Crear carpetas organizadas por fecha

### 📁 Ejemplo en S3

```plaintext
backup-bucket/
│
├── 2026-04-10/
│   ├── archivo1.txt
│   ├── archivo2.jpg
│
├── 2026-04-11/
│   ├── archivo3.txt
```

---

## 3. Monitor de instancias EC2

### 🎯 Objetivo

Visualizar el estado de instancias EC2.

### ⚙️ Información mostrada

* Instance ID
* Estado
* Tipo de instancia
* IP pública

---

## 4. Script para limpiar buckets S3 automáticamente

### 🎯 Objetivo

Eliminar archivos antiguos en S3.

### ⚙️ Funcionalidades

* Listar objetos
* Detectar archivos con más de 30 días
* Eliminarlos automáticamente

---

## 5. Sistema simple de alertas con CloudWatch

### 🎯 Objetivo

Crear métricas personalizadas desde Python.

### ⚙️ Funcionalidades

* Enviar métricas personalizadas
* Integración con alarmas de CloudWatch

---

## 6. Generador automático de usuarios IAM

### 🎯 Objetivo

Automatizar la creación de usuarios IAM.

### ⚙️ Funcionalidades

* Crear usuarios
* Asignar políticas
* Generar access keys

---

## 7. Inventario de recursos AWS

### 🎯 Objetivo

Generar un inventario de recursos AWS.

### 🛠️ Servicios utilizados

* EC2
* S3
* Lambda

### 📤 Salida

```json
aws_inventory.json
```

---

## 📌 Notas

* Asegúrate de tener permisos adecuados en AWS para cada servicio.
* Se recomienda usar roles IAM en lugar de credenciales hardcodeadas.

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas.
Puedes hacer fork del proyecto y enviar un pull request.

---

## 📄 Licencia

Este proyecto está bajo la licencia MIT.
