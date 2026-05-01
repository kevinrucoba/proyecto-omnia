# 🎵 Omnia - Plataforma de Streaming (Cloud Native)

Bienvenido al repositorio oficial de **Omnia**, una plataforma de streaming de audio diseñada bajo una arquitectura de microservicios y nativa de la nube (Cloud Native). 

Este proyecto demuestra la implementación de un ecosistema escalable y altamente disponible utilizando orquestación de contenedores, gestión de paquetes e integración/entrega continua (CI/CD).

## 🏗️ Arquitectura de Microservicios

La plataforma está dividida en tres microservicios principales, cada uno encapsulado en su propio contenedor para garantizar aislamiento y escalabilidad independiente:

*   **🔐 Omnia-Auth:** Gestión de identidades, sesiones de usuarios y validación de suscripciones premium.
*   **📚 Omnia-Catalog:** Motor de búsqueda y gestión de metadatos (artistas, álbumes, listas de reproducción).
*   **🎧 Omnia-Stream:** Procesamiento crítico y entrega de archivos binarios de audio con baja latencia.

## 🛠️ Stack Tecnológico

*   **Orquestación:** Kubernetes (K8s)
*   **Contenedorización:** Docker
*   **Gestión de Paquetes:** Helm
*   **CI/CD:** GitHub Actions

## 📂 Estructura del Proyecto

El repositorio está organizado separando el código fuente de las definiciones de infraestructura:
```text
proyecto-omnia-k8s/
├── omnia-auth/                 # Código fuente del microservicio Auth
├── omnia-catalog/              # Código fuente del microservicio Catalog
├── omnia-stream/               # Código fuente del microservicio Stream
├── charts/                     
│   └── omnia-chart/            # Helm Chart para despliegue en K8s
└── .github/                    
    └── workflows/              # Pipeline de Integración y Entrega Continua
