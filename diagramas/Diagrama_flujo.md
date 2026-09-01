```mermaid
flowchart TD
    A([INICIO]) --> B[/Registrar/]
    B --> C{¿Datos completos?}

    C -- Sí --> D{¿El correo existe?}
    C -- No --> E[Mostrar datos faltantes]

    D -- Sí --> G[Advertencia]
    D -- No --> H[Registro]

    G --> F([FIN])
    E --> F
    H --> F 
    ```
