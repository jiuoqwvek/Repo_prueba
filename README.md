# Proyecto: Sincronización Inteligente de Inventario (Caso: Unimarc)

---

### 1. Introducción
Este repositorio contiene el desarrollo de una solución integral basada en agentes LLM y pipelines RAG, aplicada al sector de retail en Chile. El proyecto busca optimizar la gestión de stock para mejorar la experiencia de usuario en plataformas de pedidos digitales.

### 2. Identificación del Problema
En cadenas como Unimarc o Santa Isabel, existe una desincronización crítica entre el stock físico de bodega y lo que el cliente ve en la aplicación.

- **Desafío:** Los productos aparecen disponibles en la app, pero están agotados en la góndola real.
- **Impacto:** Pérdida de ventas, frustración del cliente y ineficiencia en el trabajo de los repartidores.
- **Causa:** Falta de un puente de información en tiempo real que procese datos de inventario y los traduzca a disponibilidad digital.

### 3. Solución con IA
Se propone un Agente Inteligente de Gestión de Existencias que utiliza:


- **Pipeline RAG (Generación Aumentada por Recuperación):** Para conectar las fuentes de datos internas (inventario de bodega) con las respuestas del modelo, asegurando precisión absoluta.
- **Agentes LLM:** Para procesar discrepancias de nombres entre sistemas y generar alertas automáticas de reposición.
- **Prompts Optimizados:** Diseñados para actuar como un gestor de tienda experto, ajustando el contenido según el requerimiento organizacional


### 4. Clonar repositorio

```bash
# 1. Clonar tu repositorio en la terminal de VS Code
git clone https://github.com/TU-USUARIO/Parcial1_Ingenier-a_de_Soluciones_con_Inteligencia_Artificial.git
# 2. Utilizar comando cd para ingresar a la carpeta
cd Parcial1_Ingenier-a_de_Soluciones_con_Inteligencia_Artificial-
```

### 5. Crear Entorno Virtual

```bash
# Crear entorno virtual
python -m venv .venv

# Activar entorno virtual
# macOS/Linux:
source .venv/bin/activate
# Windows:
.venv\Scripts\activate
```

### 6. Instalar Dependencias

```bash
#  Necesario tener archivo de requirements.txt incluido en la carpeta
pip install -r requirements.txt
```

### 7. Configurar Variables de Entorno

```bash
# Copiar el archivo de ejemplo
cp .env.example .env
```

Edita el archivo `.env` con tus credenciales:

```env
OPENAI_BASE_URL="https://models.inference.ai.azure.com"
GITHUB_BASE_URL="https://models.inference.ai.azure.com"
OPENAI_EMBEDDINGS_URL="https://models.github.ai/inference"
GITHUB_TOKEN="tu_github_token_aqui"
LANGSMITH_TRACING="true"
LANGSMITH_API_KEY="tu_langsmith_api_key_aqui"
LANGSMITH_PROJECT="ingenieria_soluciones_con_ia"
```
