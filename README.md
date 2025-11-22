
# 📘 README – Aplicación Cloud Native (2025)
### **Fullstack + Serverless Web App usando AWS Amplify (Edición 2025)**  
**Autor:** Edwin Ramos  
**Actualizado:** Enero 2025  

---

## 🧭 1. Introducción
Este proyecto implementa una **aplicación nativa en la nube** siguiendo una arquitectura completamente **serverless**, modernizada para el stack tecnológico de **2025**, incluyendo:

- **Frontend:** React 18 + Amplify UI  
- **Backend:** AWS Lambda (Node.js 20 + ARM64 + SnapStart)  
- **API:** Amazon API Gateway (HTTP API v2)  
- **Base de Datos:** DynamoDB (diseño de tabla única + GSIs)  
- **Almacenamiento:** Amazon S3  
- **Orquestación:** AWS Amplify Gen 2  

Este repositorio fue modernizado a partir del proyecto *AmplifyWorkshop* y adaptado para cumplir con evaluaciones técnicas actuales relacionadas con arquitectura cloud-native.

---

## 🎯 2. Objetivo del Proyecto

| Requerimiento | Descripción |
|--------------|-------------|
| **Frontend** | Interfaz web React 18 servida desde S3 + CloudFront |
| **Backend** | Servicios sin servidor expuestos mediante API Gateway + Lambda |
| **Base de Datos** | DynamoDB con consultas optimizadas y escalabilidad automática |
| **Almacenamiento de Objetos** | S3 para imágenes y contenido estático |

---

## 🧱 3. Tecnologías Actualizadas (2025)

### 🔹 Frontend
- React 18  
- Amplify UI React v5  
- CRA 5 / Vite compatible  
- CloudFront NextGen  
- Edge Functions para optimización de cache y seguridad  

### 🔹 Backend
- Lambda con Node.js 20  
- Arquitectura ARM64  
- SnapStart para arranques ultrarrápidos  
- API Gateway HTTP API (v2)

### 🔹 Base de Datos
- DynamoDB  
- GSIs  
- TTL automático  
- SDK AWS v3

### 🔹 Storage
- S3 (privado + público)  
- Amplify Storage v2  
- Presigned URLs v4  

---

## 🏗 4. Arquitectura Cloud 2025

```
Usuario ─► Navegador (React + Amplify)
         └► CloudFront
             └► S3 (Static Hosting)
                 └► API Gateway HTTP API
                     └► AWS Lambda (Node20, ARM64)
                        ├► DynamoDB
                        └► S3 (Object Storage)
```

---

## 🔄 5. Flujo de Funcionamiento

1. El usuario navega la aplicación React servida por CloudFront.  
2. El frontend se comunica con el backend usando AWS Amplify.  
3. API Gateway enruta las solicitudes a Lambda.  
4. Lambda ejecuta la lógica del negocio.  
5. DynamoDB persiste los datos.  
6. S3 almacena archivos e imágenes.  

---

## 🛠 6. Instalación y Ejecución

### Requisitos
- Node.js 20+  
- AWS CLI configurado  
- Amplify CLI v12+  

### Instalar dependencias
```bash
npm install
```

### Ejecutar localmente
```bash
npm start
```

### Desplegar en AWS
```bash
amplify init
amplify push
amplify publish
```

---

## 🗄 7. Estructura del Proyecto

```
├── amplify/               
├── public/              
├── src/                  
├── package.json
└── README.md
```

---

## 📎 8. Justificación Técnica

- **Amplify Gen 2** permite IaC moderna basada en TypeScript.  
- **Lambda + ARM64** reduce costos y aumenta rendimiento.  
- **API Gateway HTTP API** es más económico y rápido que REST API.  
- **DynamoDB** escala automáticamente para millones de solicitudes.  
- **S3 + CloudFront** es el estándar mundial para hosting web.  

---

## 📄 9. Licencia
MIT License.

