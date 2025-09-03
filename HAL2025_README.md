# HAL2025 – El Asistente Virtual del Futuro

## 🚀 Sobre el proyecto
HAL2025 está pensado para ser el mejor asistente virtual de nueva generación.  
En esta primera fase utiliza **n8n** como motor de automatización y una base de datos **Postgres**.  
El objetivo es crecer poco a poco, añadiendo flujos de automatización inteligentes, integraciones y nuevas funciones.

---

## ⚙️ Instalación

1. **Clona o descarga este repositorio.**  
2. **Crea tu archivo `.env`.** Hay un archivo de ejemplo (`.env_example`) que puedes copiar y modificar según tus necesidades.  

Ejemplo de `.env`:

```env
# --- Postgres ---
POSTGRES_USER=n8n
POSTGRES_PASSWORD=supersegura_cambia_esto
POSTGRES_DB=n8n

# --- n8n host/protocol (ajusta si tienes dominio/https) ---
N8N_PROTOCOL=http
N8N_HOST=localhost
WEBHOOK_URL=http://localhost:5678/

# --- Auth básica para el primer arranque ---
N8N_BASIC_AUTH_USER=admin
N8N_BASIC_AUTH_PASSWORD=cambia_esto_tambien

# --- Clave de cifrado (32 bytes hex) ---
# Genera una nueva con:  openssl rand -hex 32
N8N_ENCRYPTION_KEY=REEMPLAZA_CON_HEX_64
```

3. **Levanta el entorno con Docker Compose:**

```bash
docker compose up -d
```

Esto instalará **n8n** junto con la base de datos **Postgres**.

---

## 🛠️ Próximos pasos
En el futuro, iremos añadiendo flujos de n8n ya listos para usar, para que puedas desplegar un asistente virtual aún más potente desde el primer minuto.

---

# HAL2025 – The Virtual Assistant of the Future

## 🚀 About the Project
HAL2025 is designed to be the next-generation virtual assistant.  
In this first phase it uses **n8n** as the automation engine and **Postgres** as its database.  
The goal is to grow steadily, adding intelligent workflows, integrations, and new features.

---

## ⚙️ Installation

1. **Clone or download this repository.**  
2. **Create your `.env` file.** There is an example file (`.env_example`) that you can copy and edit.  

Example `.env`:

```env
# --- Postgres ---
POSTGRES_USER=n8n
POSTGRES_PASSWORD=supersecure_change_this
POSTGRES_DB=n8n

# --- n8n host/protocol (adjust if you have domain/https) ---
N8N_PROTOCOL=http
N8N_HOST=localhost
WEBHOOK_URL=http://localhost:5678/

# --- Basic auth for the first run ---
N8N_BASIC_AUTH_USER=admin
N8N_BASIC_AUTH_PASSWORD=change_this_too

# --- Encryption key (32 bytes hex) ---
# Generate a new one with:  openssl rand -hex 32
N8N_ENCRYPTION_KEY=REPLACE_WITH_HEX_64
```

3. **Start the environment with Docker Compose:**

```bash
docker compose up -d
```

This will install **n8n** together with the **Postgres** database.

---

## 🛠️ Next Steps
In the future, we will provide ready-to-use n8n flows so you can deploy an even more powerful virtual assistant from the very beginning.
