# Analisis de un Sistema de Plataforma Educativa en Línea 

# Código:
flowchart TB
    %% Entorno externo al sistema
    subgraph Entradas
        Usuarios[Usuarios]
        Profesor[Profesor]
        Administrador[Administrador]
    end

    %% Sistema
    subgraph Sistema
        A[Entradas: Registro de usuarios, carga de cursos, configuración del sistema]
        B[Procesos: Gestión de cursos, evaluaciones, foros, clases virtuales, calificaciones, administración]
        C[Salidas: Cursos disponibles, evaluaciones aplicadas, calificaciones, certificados, reportes]
        D[Retroalimentación: Evaluaciones de cursos, comentarios en foros, métricas de desempeño]
    end

    %% Flujo del sistema
    Usuarios --> A
    Profesor --> A
    Administrador --> A
    A --> B
    B --> C
    C --> D

    %% Retroalimentación hacia los procesos
    D --> B

    %% Salidas afectan al entorno
    C --> Usuarios
    C --> Profesor
    C --> Administrador

## Grupo: 
Santiago Arenas Rios
Julian Andres Arbelaez Rios
David Giraldo Henriet
