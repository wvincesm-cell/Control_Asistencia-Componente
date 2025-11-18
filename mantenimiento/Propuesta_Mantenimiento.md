Propuesta de Mantenimiento Perfectivo para “Control_Asistencia”
1. Introducción

Objeto: Proponer un plan de mantenimiento perfectivo para el sistema de control de asistencia alojado en el repositorio GitHub indicado, con el propósito de mejorar su calidad, agregar nuevas funcionalidades y optimizar su desempeño.

Justificación: Según datos de ingeniería de software, el mantenimiento perfectivo representa un porcentaje muy alto del esfuerzo de mantenimiento (varios autores estiman ~ 60 %) porque se centra en mejorar la eficiencia y funcionalidad del sistema. 
Ingeniería de Software III
+2
Apuntes & Cursos
+2

También se considera una práctica recomendada por normas de mantenimiento de software. 
Grupo Alarcos
+1

2. Objetivos

Mejorar el rendimiento del sistema de control de asistencia (tiempos de respuesta, consumo de recursos).

Agregar nuevas funcionalidades útiles para los usuarios finales (por ejemplo, reportes avanzados, notificaciones, exportación de datos).

Optimizar la mantenibilidad del código (refactorización, limpieza del código, mejorar documentación).

Incrementar la usabilidad de la interfaz, para que sea más intuitiva y fácil de manejar por los responsables del control de asistencia.

Garantizar la calidad de los cambios mediante pruebas (unitarias, de integración).

3. Alcance del mantenimiento

Este plan de mantenimiento no incluye:

Corrección de bugs críticos (mantenimiento correctivo).

Adaptación a cambios del entorno tecnológico (como migrar a una nueva plataforma): eso sería mantenimiento adaptativo. 
Wikipedia

Mantenimiento preventivo enfocado en reestructuración para evitar futuros errores, aunque algunas refactorizaciones podrían entrar dentro si ayudan a la mantenibilidad.

En cambio, sí se incluyen:

Refactorización de módulos actuales para mejorar su rendimiento.

Implementación de nuevas historias de usuario / características.

Mejora de la arquitectura interna, si es necesario, para facilitar futuras evoluciones.

Mejoramiento de la documentación técnica (README, comentarios, wiki) y documentación para usuarios.

4. Actividades específicas propuestas

Aquí algunas tareas concretas que podríamos llevar a cabo bajo el mantenimiento perfectivo:

Análisis de rendimiento actual: Medir tiempos de respuesta, uso de memoria, cuellos de botella.

Refactorización de componentes: Identificar partes del código que pueden mejorarse para ganar eficiencia o legibilidad.

Implementación de nuevas funcionalidades:

Reportes de asistencia más avanzados (por mes, por persona, estadísticas).

Exportar datos (CSV, Excel, PDF).

Alertas o notificaciones (por ejemplo, enviar un email si un usuario no se registra durante varios días).

Dashboard (panel) para supervisores con métricas de control de asistencia.

Optimización de base de datos: Si hay una base de datos, optimizar consultas, índices, relaciones para que las operaciones sean más rápidas.

Mejoras en la interfaz de usuario (UI): Rediseño de pantallas para hacerlas más intuitivas.

Documentación:

Actualizar el README.md con una guía de uso y configuración.

Crear o mejorar la documentación del API (si aplica).

Documentar el architecture design, flujos y dependencias.

Pruebas: Crear/expandir tests unitarios, de integración y pruebas de rendimiento para validar los cambios.

Despliegue de versiones: Planificar lanzamientos trimestrales o semestrales con las mejoras, para que los usuarios puedan beneficiarse sin interrumpir mucho el servicio.

5. Cronograma

Propuesta de cronograma (6 meses):

Fase	Actividades principales	Duración estimada
Fase 1 – Diagnóstico	Medición de rendimiento, auditoría del código, identificación de funcionalidades prioritarias	1 mes
Fase 2 – Planificación	Definir backlog de mejoras, priorizar historias, diseñar arquitectura/refactorización	1 mes
Fase 3 – Implementación	Desarrollo de nuevas funciones, refactorización, optimización de DB	2–3 meses
Fase 4 – Pruebas	Pruebas unitarias, integración, rendimiento	1 mes
Fase 5 – Documentación	Actualización de manuales, README, wiki	0.5 mes
Fase 6 – Despliegue y revisión	Lanzamiento de nueva versión, feedback de usuarios, ajustes finales	0.5 mes
6. Recursos necesarios

Equipo de desarrollo: 1-2 desarrolladores con conocimiento del repositorio, preferiblemente con experiencia en refactorización y optimización.

Infraestructura: entorno de desarrollo, pruebas y staging; si se va a hacer análisis de rendimiento, herramientas para medir (profiler, herramientas de monitoreo).

Tiempo estimado: según el cronograma; también tiempo para code reviews y reuniones de seguimiento.

Usuarios o stakeholders: para definir qué nuevas funcionalidades son más urgentes o útiles.

7. Beneficios esperados

Mejora del rendimiento: el sistema será más rápido y eficiente, lo que mejora la experiencia del usuario.

Nuevas funcionalidades: los usuarios podrán aprovechar nuevas herramientas como reportes y exportaciones.

Mejor mantenibilidad: el código será más claro, modular y fácil de modificar en el futuro, lo que reduce el costo de futuros cambios.

Calidad: con buenas pruebas, se reduce el riesgo de introducir errores.

Valor a largo plazo: al invertir en mejoras evolutivas, el sistema se mantiene relevante y útil, lo que prolonga su vida útil y evita abandono o reconstrucción desde cero.

8. Riesgos y mitigaciones

Riesgo: Introducir nuevas funciones podría generar bugs.
Mitigación: asegurarse de tener un buen suite de pruebas automatizadas y pruebas manuales antes del despliegue.

Riesgo: Refactorización extensa puede retrasar otras tareas.
Mitigación: dividir la refactorización en partes pequeñas y priorizadas; usar revisiones de código frecuentes.

Riesgo: Falta de alineación con usuarios: que la nueva funcionalidad no sea la más útil.
Mitigación: involucrar a los usuarios clave desde la fase de planificación para definir prioridades.

Riesgo: Costos de tiempo y recursos.
Mitigación: estimar claramente el trabajo, hacer entregas parciales y revisar los resultados con el equipo para ajustar según sea necesario.

9. Métricas de éxito

Para asegurar que el mantenimiento perfectivo está siendo efectivo, se pueden usar las siguientes métricas:

Tiempo de respuesta antes y después (medir latencia, rendimiento).

Uso de memoria / recursos en producción.

Número de usuarios que usan las nuevas funciones (reportes, exportaciones, dashboards).

Cobertura de pruebas (unitarias, integración).

Frecuencia de commits relacionados al refactor (indicador de que el código se está volviendo más manejable).

Feedback de usuarios: encuestas o entrevistas para saber si encuentran útiles las mejoras.

10. Conclusión

El mantenimiento perfectivo no solo es una práctica recomendable sino esencial para que un sistema como Control_Asistencia-Componente continúe siendo útil y competitivo. La propuesta aquí presentada busca no solo mejorar el rendimiento y la usabilidad, sino también preparar el sistema para futuras evoluciones, asegurando que el código se mantenga limpio, documentado y probado.
