# 🎬 Sistema de Recomendación de Series basado en Grafos

## 📖 Descripción
Este proyecto implementa un sistema de recomendación de series utilizando un enfoque híbrido basado en **filtrado colaborativo** y **grafos**. El objetivo es mejorar la experiencia del usuario en plataformas de streaming mediante recomendaciones personalizadas y relevantes.

El sistema modela usuarios, series y géneros como un grafo, permitiendo descubrir relaciones complejas y generar sugerencias más precisas que los métodos tradicionales.

---

## 🎯 Objetivos
- Reducir la sobrecarga de información
- Mejorar la personalización de recomendaciones
- Facilitar la toma de decisiones del usuario
- Aprovechar estructuras de grafos para detectar patrones ocultos

---

## 🧠 Enfoque del Sistema
El sistema combina:

- 🔹 **Filtrado Colaborativo**
- 🔹 **Filtrado Basado en Contenido**
- 🔹 **Modelo basado en Grafos**

---

## 🧩 Modelo de Datos (Grafo)

### 🔸 Nodos
- `Usuario {id, nombre}`
- `Serie {id, nombre}`
- `Género {nombre}`

### 🔸 Relaciones
- `(Usuario)-[:VIO]->(Serie)`
- `(Usuario)-[:GUSTO]->(Serie)`
- `(Usuario)-[:QUIERE_VER]->(Serie)`
- `(Serie)-[:PERTENECE]->(Género)`

---

## ⚙️ Funcionamiento

1. El usuario selecciona series de interés  
2. El sistema analiza sus preferencias  
3. Se identifican usuarios similares  
4. Se obtienen series vistas por usuarios similares  
5. Se filtran las series no vistas  
6. Se generan recomendaciones ordenadas  

---

## 🛠️ Tecnologías Utilizadas

- **Neo4j** – Base de datos de grafos  
- **Cypher** – Lenguaje de consulta  
- *(Agrega aquí tu stack: Python, JavaScript, etc.)*

---

## 📊 Algoritmos Implementados

- 🔸 K-Nearest Neighbors (KNN)
- 🔸 Random Walk
- 🔸 PageRank adaptado

---

## 🚀 Instalación

### 1. Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo