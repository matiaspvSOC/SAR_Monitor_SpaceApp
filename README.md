# SAR Monitor — Región del Biobío
**Monitoreo satelital de inundaciones y cuerpos de agua mediante Radar de Apertura Sintética (SAR)**

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![HTML5](https://img.shields.io/badge/Frontend-HTML%20%2F%20JS-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

> **Demo interactiva en vivo:** (https://matiaspvsoc.github.io/SAR_Monitor_SpaceApp/) 

---

## El Problema: ¿Por qué Radar (SAR) y no satélites ópticos?

Durante sistemas frontales e inundaciones en el sur de Chile (Región del Biobío), la cobertura nubosa bloquea por completo la visión de los satélites ópticos tradicionales durante semanas, impidiendo evaluar zonas afectadas en tiempo real.

---

<img width="512" height="444" alt="nasa-worldview-2024 JUN 01-to-2024 JUL 01" src="https://github.com/user-attachments/assets/c1b91e76-2ca2-4817-85c9-f9c40606810a" />

**Evidencia en terreno (30 días consecutivos de nubosidad sobre la zona de estudio):**
[Uploading nasa-worldview-2024 JUN 01-to-2024 JUL 01.gif…]()


A diferencia de los sensores ópticos, el **Radar de Apertura Sintética (SAR)** emite sus propias microondas, atravesando las nubes y operando tanto de día como de noche para detectar cambios en la superficie del agua.

---

## Vista Previa de la Plataforma Web

El proyecto procesa datos satelitales y los exporta a una interfaz web ligera donde es posible alternar capas geoespaciales y analizar puntos de control:

<img width="1868" height="883" alt="imagen" src="https://github.com/user-attachments/assets/e30c1d06-b86f-4db2-8e96-9a97aa10bf02" />

---

<img width="1867" height="888" alt="imagen" src="https://github.com/user-attachments/assets/95ac7d7b-92fe-4b1b-9681-d6d87082a861" />


---

## Arquitectura y Estructura del Repositorio

El flujo de trabajo separa el procesamiento geoespacial en Python de la visualización web estática:

```text
SAR_Monitor_SpaceApp/
├── analisis.ipynb    # Limpieza, procesamiento de bandas SAR y extracción de métricas
├── EC_mapa.csv       # Dataset procesado con coordenadas y registros de monitoreo
├── capas/            # Capas geoespaciales generadas para superposición en el mapa
├── index.html        # Visor web interactivo desplegado en GitHub Pages
└── LICENSE           # Licencia MIT
