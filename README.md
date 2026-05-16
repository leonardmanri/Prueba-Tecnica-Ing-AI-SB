# Sistema de Triaje Visual - Solucion End-to-End para Patologias en Vid

## Descripcion General
Este repositorio contiene la respuesta integral a la prueba tecnica para el rol de IA. El proyecto aborda la problematica fitosanitaria en cultivos de uva mediante un enfoque de Inteligencia Artificial en el Borde (Edge AI), transformando predicciones de Machine Learning en reglas de negocio accionables para optimizar la operacion en campo.

El entregable esta dividido de forma metodologica en dos componentes estrategicos:

1. **Core Tecnico (`/nucleo_tecnico`):** Pipeline de ingenieria de datos, entrenamiento del modelo optimizado en Recall (YOLOv8 Nano), capa de aplicacion con OpenCV para la matriz de riesgo y MVP interactivo implementado en Gradio.
2. **Estrategia de Negocio (`/estrategia_negocio`):** Roadmap de despliegue operacional, analisis de mitigacion de riesgos (Domain Shift), justificacion del ROI y el enlace a la video-presentacion ejecutiva de la propuesta.

## Estructura de Navegacion

* Para evaluar el codigo, las metricas de entrenamiento y ejecutar el prototipo interactivo en Google Colab, dirijase a: [Documentacion Tecnica e Instrucciones de Ejecucion](./nucleo_tecnico/README.md).
* Para revisar la viabilidad comercial, las fases de despliegue en campo y acceder al video de sustentacion, dirijase a: [Propuesta de Despliegue de Negocio](./estrategia_negocio/Propuesta_Despliegue_Negocio.md).

## Supuesto Macro de Diseño
La solucion asume que el entorno de despliegue final presenta restricciones severas de conectividad red (zonas rurales). Por ende, toda la arquitectura se diseno bajo el paradigma de Edge Computing, garantizando que la inferencia pueda ejecutarse al 100% sin depender de peticiones HTTP a la nube durante la operacion critica del jornalero.
