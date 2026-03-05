# Kestra

## Configuración previa al arranque

El ejemplo realizado utiliza un API Key de Google AI Studio. Se puede solicitar una cuenta gratuita que proporciona 20 consultas al día.

El valor de dicho secreto debe ser codificado en base64 y setado en el fichero docker compose.

```bash
echo -n "mi-api-key" | base64
bWktYXBpLWtleQ==
```

```yaml
    environment:
      SECRET_GEMINI_API_KEY: "bWktYXBpLWtleQ=="
```

## Arranque de la herramienta

```bash
docker compose up -d
```

Acceso en [http://localhost:8080](http://localhost:8080)

## Carga del flow de ejemplo

Una vez arrancado el entorno, entrar en la sección Flow e importar el flujo *simple_sumarize_agent* contenido en el directorio flow. 

