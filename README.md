# aws-stude-chatbot
Serverless 3-Tier Architecture Chatbot with Amazon Bedrock, S3 Vectors, DynamoDB, API Gateway, Lambda, and Cognito.
# 🤖 AWS Study Chatbot (Serverless 3-Tier Architecture)

Este proyecto implementa un **chatbot de estudio para certificaciones AWS**, diseñado con una **arquitectura 3-Tier serverless**, de bajo costo y fácil de mantener.  

El chatbot responde preguntas usando tus propios documentos de estudio (almacenados en S3), y aprovecha **Amazon Bedrock Knowledge Bases con S3 Vectors** para entregar respuestas basadas en **RAG (Retrieval-Augmented Generation)**.

---

## 🏗️ Arquitectura 3-Tier

- **Presentation Tier (Frontend):**  
  Aplicación web estática en **S3 + CloudFront** (desplegada desde GitHub).  

- **Application Tier (Backend):**  
  **API Gateway + Lambda**, que conecta con **Amazon Bedrock** para procesar las consultas.  

- **Database Tier (Persistencia):**  
  - **Amazon S3 + Vectors** → documentos de estudio vectorizados para el RAG.  
  - **Amazon DynamoDB** → historial de conversaciones cuando el usuario inicia sesión (con Cognito).  

---

## 🔹 Características
- ✅ Chatbot de estudio con respuestas personalizadas.  
- ✅ Interfaz web accesible (sin login obligatorio).  
- ✅ Opción de iniciar sesión con Cognito para guardar historial.  
- ✅ Persistencia en DynamoDB.  
- ✅ Arquitectura serverless → bajo costo y escalable.  

---

## 📂 Estructura del proyecto
