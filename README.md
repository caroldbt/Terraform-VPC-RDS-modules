# Proyecto de Infraestructura en AWS con Terraform

## Descripción

Este proyecto configura la infraestructura en AWS utilizando Terraform. Se implementa una VPC, una instancia de cómputo y una base de datos, asegurando buenas prácticas y modularización del código para facilitar su mantenimiento y escalabilidad.

## Requisitos

Antes de comenzar, asegúrate de tener instaladas las siguientes herramientas en tu sistema:

1. [Terraform](https://www.terraform.io/downloads.html) - Herramienta para definir y aprovisionar infraestructura utilizando código.
2. [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) - Interfaz de línea de comandos de AWS para gestionar recursos de AWS.

## Estructura del Proyecto

El proyecto está organizado en la siguiente estructura de directorios:

```
terraform/
├── main.tf
├── variables.tf
├── outputs.tf
└── modules/
├── vpc/
│ ├── main.tf
│ ├── variables.tf
│ └── outputs.tf
├── compute/
│ ├── main.tf
│ ├── variables.tf
│ └── outputs.tf
└── basedatos/
├── main.tf
├── variables.tf
└── outputs.tf
```
## Instrucciones de Uso

### Paso 1: Clonar el Repositorio

Clona este repositorio en tu máquina local.

```sh
git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_DIRECTORIO>
```
### Paso 2: Configurar AWS CLI
Inicia sesión en tu cuenta de AWS utilizando AWS CLI.
```
aws configure
```
### Paso 3: Inicializar Terraform
Inicializa el entorno de trabajo de Terraform.
```
terraform init
```
### Paso 4: Planificar la Infraestructura
Revisa el plan de implementación para asegurarte de que los recursos se crearán correctamente.
```
terraform plan
```
### Paso 5: Aplicar la Configuración
Aplica la configuración de Terraform para crear los recursos en AWS.
```
terraform apply
```
