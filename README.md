# Trabajo_final_modulo3
Trabajo_final_modulo3 

Descripción
Este repositorio contiene la documentación técnica, diseño de arquitectura y especificaciones de API para el nuevo sistema de administración de contratos. El objetivo es centralizar la "fuente de verdad" del proyecto, asegurando trazabilidad y estándares de calidad profesional.
Objetivos de la Documentación
    Estandarización: Definir contratos de API claros bajo el estándar OpenAPI (Swagger).
    Transparencia: Registrar cada fase del diseño (Diagramas, Entidad-Relación).
    Trazabilidad: Mantener un histórico de decisiones técnicas (ADR).
Estructura del Repositorio
La documentación se organiza de la siguiente manera para facilitar la auditoría del avance:
Plaintext

├── 📂 docs

│   ├── 📂 architecture       # Diagramas C4, Flujos de Secuencia y ERD.

│   ├── 📂 api-contracts      # Archivos YAML/JSON (OpenAPI Spec).

│   ├── 📂 adr                # Architectural Decision Records (Decisiones clave).

│   └── 📂 business-rules     # Lógica de negocio y validación de contratos.

├── 📂 resources              # Assets, imágenes y prototipos de UI.

└── README.md                 # Guía principal (este archivo).

Especificaciones de la API (Contratos)
El diseño de la comunicación entre servicios se basa en el principio API-First.
Recurso	Método	Endpoint	Descripción	Estado
Auth	POST	/api/v1/auth/login	Autenticación de usuarios.	
Contratos	GET	/api/v1/contracts	Listado de contratos activos.	
Contratos	POST	/api/v1/contracts	Creación de nuevo contrato.	

Diseño del Sistema
Para garantizar la escalabilidad, se han definido los siguientes artefactos:
    Modelo de Datos: Diseño relacional optimizado para la integridad de los contratos legales.
    Arquitectura: Basada en capas (Controller, Service, Repository).
    Seguridad: Implementación de JWT para la protección de los endpoints.
📈 Cronograma de Entregas (Roadmap)
Para asegurar el cumplimiento de la fecha de entrega de la práctica, se sigue este calendario de hitos:
    [ ] Fase 1: Levantamiento de requerimientos y Casos de Uso. 
    [ ] Fase 2: Diseño del Contrato de API (OpenAPI v3). 
    [ ] Fase 3: Diagrama Entidad-Relación y Diccionario de Datos.
    [ ] Fase 4: Revisión final y congelación de documentación.
👥 Colaboradores y Control de Versiones
Cada avance en este repositorio debe seguir el flujo de trabajo GitFlow:
    main: Versiones estables para entrega.
    develop: Integración de nuevas funcionalidades.
    docs/feature-name: Ramas específicas para redactar documentación nueva.
