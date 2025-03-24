# Definición de Requerimientos

## Definición de Requerimientos de Usuario

Los requerimientos de usuario se derivan de las necesidades y expectativas identificadas en la investigación con los distintos perfiles de usuarios del sistema. Se centran en garantizar accesibilidad, eficiencia y facilidad de uso en la digitalización de expedientes clínicos.

## Definición de Tipos de Requerimientos

Se establecen dos tipos principales de requerimientos:

- **Requerimientos Funcionales:** Especifican las acciones y procesos que el sistema debe permitir a los usuarios realizar.
- **Requerimientos No Funcionales:** Se refieren a aspectos como la usabilidad, seguridad, rendimiento y accesibilidad del sistema.

## Requerimientos Funcionales

**RF-1:** El sistema debe permitir a los terapeutas en formación registrar y consultar expedientes clínicos.

**RF-2:** El sistema debe poder permitir que los coordinadores puedan revisar y aprobar los registros de los terapeutas.

**RF-3:** El sistema debe permitir que la secretaría gestione citas y los cambios hechos sean notificados automáticamente a terapeutas y pacientes.

**RF-4:** El sistema debe permitir que el personal de TI tenga acceso a la gestión de seguridad y mantenimiento del sistema.

**RF-5:** El sistema debe permitir la asignación de casos a un determinado terapeuta y supervisor.

**RF-6:** El sistema debe permitir mantener un historial de sesiones con reportes adjuntos.

**RF-7:** El sistema debe permitir la evaluación del servicio al finalizar un tratamiento.

**RF-8:** El sistema debe permitir el registro y almacenamiento de pruebas psicológicas (psicodiagnóstico, orientación vocacional).

**RF-9:** El sistema debe permitir la gestión de documentos adicionales según el tipo de tratamiento.

**RF-10:** El sistema debe permitir controlar el acceso a los expedientes según el rol del usuario (terapeuta, supervisor, coordinador, secretario).

**RF-11:** El sistema debe permitir restringir el acceso a expedientes a terapeutas asignados y supervisores.

**RF-12:** El sistema debe permitir registrar auditorías de acceso (quién visualizó o editó un expediente).

**RF-13:** El sistema debe permitir implementar permisos para roles específicos (coordinación, secretaría, supervisores, terapeutas, becarios).

**RF-14:** El sistema debe permitir proteger la información contra modificaciones no autorizadas.

**RF-15:** El sistema debe permitir registrar y programar sesiones entre terapeutas y pacientes.

**RF-16:** El sistema debe permitir que los terapeutas agreguen notas de sesión estructuradas.

**RF-17:** El sistema debe permitir ofrecer plantillas personalizables para reportes de sesiones.

**RF-18:** El sistema debe permitir generar y almacenar reportes de evaluación psicológica.

**RF-19:** El sistema debe permitir gestionar la historia clínica del paciente según las guías establecidas.

**RF-20:** El sistema debe permitir la carga de documentos en diferentes formatos (PDF, imágenes escaneadas).

**RF-21:** El sistema debe permitir la gestión de la finalización de casos y marcar expedientes como cerrados.

**RF-22:** El sistema debe permitir mantener los expedientes almacenados por 5 años antes de su eliminación.

**RF-23:** El sistema debe permitir notificar a los terapeutas sobre documentos pendientes de entrega.

**RF-24:** El sistema debe permitir la comunicación entre secretaría y terapeutas para validaciones.

**RF-25:** El sistema debe permitir registrar cambios en la asignación de terapeutas en casos de transferencia.

**RF-26:** El sistema debe permitir la digitalización de documentos físicos mediante escaneo.

**RF-27:** El sistema debe permitir la carga y asociación de imágenes de pruebas psicológicas (dibujos, protocolos).

**RF-28:** El sistema debe permitir la integración de herramientas de procesamiento de texto para la redacción de reportes.

**RF-29:** El sistema debe permitir mantener una base de datos de motivos de consulta para estadísticas.

## Requerimientos No Funcionales Relacionados con IHC

### Usabilidad

**RNF-1:** El sistema debe permitir la consulta y actualización de expedientes en un tiempo máximo de 5 minutos, medido desde el inicio de la sesión hasta la confirmación del cambio. 

**RNF-2:** La interfaz debe ser intuitiva para nuevos usuarios, con un tiempo de aprendizaje menor a 2 días. Se logrará mediante: 

    - Un tutorial interactivo en el primer acceso. 

    - Un sistema de ayuda contextual con instrucciones específicas según la sección. 

    - Indicaciones visuales para errores o acciones incompletas. 

**RNF-3:** La organización de la información debe seguir una jerarquía clara: 

    - Datos personales del paciente en la parte superior. 

    - Historial clínico accesible en pestañas o secciones colapsables. 

    - Opciones de acción destacadas con colores diferenciados (ejemplo: verde para confirmar, rojo para eliminar). 

### Seguridad

**RNF-4:** Se debe asegurar la confidencialidad de la información de los pacientes mediante un nivel de seguridad que cumpla con estándares de cifrado de al menos AES-256 en la base de datos 

**RNF-5:** Se debe aplicar control de acceso basado en roles (RBAC), asegurando que cada usuario solo pueda acceder a la información necesaria según su función. 

**RNF-6:** El sistema debe cumplir con normativas éticas y legales de confidencialidad, como la Ley General de Protección de Datos Personales en Posesión de Sujetos Obligados (LGPDPPSO) y Normas ISO/IEC 27001 en gestión de seguridad de la información. 

**RNF-7:** El sistema debe garantizar la seguridad de las sesiones de usuario mediante la protección contra accesos no autorizados. En caso de inactividad de más de 15 minutos, el sistema cerrará la sesión automáticamente y requerirá reautenticación. 

### Rendimiento

**RNF-8:** El sistema debe ser capaz de gestionar múltiples consultas simultáneamente sin degradar la experiencia del usuario, optimizando la ejecución de consultas a la base de datos. 

**RNF-9:** El tiempo de respuesta en la carga y consulta de expedientes no debe exceder los 2 segundos en condiciones normales de operación. 

**RNF-10:** El sistema debe soportar el acceso concurrente de múltiples usuarios sin afectar la velocidad de procesamiento. 

**RNF-11:** Se debe utilizar una arquitectura escalable con balanceo de carga que permita soportar la demanda de las consultas. 

### Portabilidad

**RNF-12:** El sistema debe ser accesible desde dispositivos móviles y computadoras, asegurando una experiencia fluida en diferentes resoluciones de pantalla. 

**RNF-13:** Debe ser compatible con múltiples navegadores web, asegurando una experiencia fluida en diferentes resoluciones de pantalla. 

**RNF-14:** El diseño debe ser responsivo: 

    - Elementos ajustables según la pantalla (ejemplo: menús desplegables en móviles). 

    - Botones de acción con un tamaño mínimo de 44x44 píxeles en dispositivos táctiles. 

    - Tipografía legible con un tamaño mínimo de 16px. 

### Mantenibilidad

**RNF-15:** El sistema debe proveer una de digitalización de documentos físicos eficiente y fácil de usar, con compatibilidad para escáneres y OCR, reduciendo el tiempo de procesamiento a un promedio de 2 minutos por documento. 

**RNF-16:** El código debe estar bien documentado y seguir estándares de desarrollo que faciliten futuras modificaciones o ampliaciones del sistema como el Javadoc. 

**RNF-17:** Se implementará una arquitectura modular que permita: 

    - La adición de nuevos módulos sin afectar el rendimiento. 

    - La actualización independiente de cada módulo sin afectar a otros. 

### Confiabilidad

**RNF-18:** El sistema debe estar disponible al menos el 99.9% del tiempo en horarios de uso frecuente (Lunes a Viernes de 9:00 - 15:00 horas), para garantizar la continuidad del servicio. 

**RNF-19:** El sistema debe tener una alta confiabilidad y tolerancia a fallos, asegurando que no se pierda información en caso de errores, y con un tiempo de recuperación inferior a 10 minutos. 

**RNF-20:** Debe contar con mecanismos de respaldo automático como Copia de seguridad y Restauración de datos en caso de falla crítica. 
