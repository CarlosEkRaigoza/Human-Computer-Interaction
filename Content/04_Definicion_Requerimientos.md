<!DOCTYPE html>
<html>
    <body>
        <h1>Definición de Requerimientos</h1>
        <h2>Definición de Requerimientos de Usuario</h2>
        <p>Los requerimientos de usuario se derivan de las necesidades y expectativas identificadas en la investigación con los distintos perfiles de usuarios del sistema. Se centran en garantizar accesibilidad, eficiencia y facilidad de uso en la digitalización de expedientes clínicos.</p>
        <h2>Definición de Tipos de Requerimientos</h2>
        <p>Se establecen dos tipos principales de requerimientos:</p>
        <ul>
            <li><strong>Requerimientos Funcionales:</strong> Especifican las acciones y procesos que el sistema debe permitir a los usuarios realizar.</li>
            <li><strong>Requerimientos No Funcionales:</strong> Se refieren a aspectos como la usabilidad, seguridad, rendimiento y accesibilidad del sistema.</li>
        </ul>
        <h2>Requerimientos Funcionales</h2>
        <ul>
            <li>El sistema debe permitir a los terapeutas en formación registrar y consultar expedientes clínicos.</li>
            <li>El sistema debe poder permitir que los coordinadores puedan revisar y aprobar los registros de los terapeutas.</li>
            <li>El sistema debe permitir que la secretaría gestione citas y los cambios hechos sean notificados automáticamente a terapeutas y pacientes.</li>
            <li>El sistema debe permitir que el personal de TI tenga acceso a la gestión de seguridad y mantenimiento del sistema.</li>
            <li>El sistema debe permitir la asignación de casos a un determinado terapeuta y supervisor.</li>
            <li>El sistema debe permitir mantener un historial de sesiones con reportes adjuntos.</li>
            <li>El sistema debe permitir la evaluación del servicio al finalizar un tratamiento.</li>
            <li>El sistema debe permitir el registro y almacenamiento de pruebas psicológicas (psicodiagnóstico, orientación vocacional).</li>
            <li>El sistema debe permitir la gestión de documentos adicionales según el tipo de tratamiento.</li>
            <li>El sistema debe permitir controlar el acceso a los expedientes según el rol del usuario (terapeuta, supervisor, coordinador, secretario).</li>
            <li>El sistema debe permitir restringir el acceso a expedientes a terapeutas asignados y supervisores.</li>
            <li>El sistema debe permitir registrar auditorías de acceso (quién visualizó o editó un expediente). </li>
            <li>El sistema debe permitir implementar permisos para roles específicos (coordinación, secretaría, supervisores, terapeutas, becarios).</li>
            <li>El sistema debe permitir proteger la información contra modificaciones no autorizadas.</li>
            <li>El sistema debe permitir registrar y programar sesiones entre terapeutas y pacientes.</li>
            <li>El sistema debe permitir que los terapeutas agreguen notas de sesión estructuradas.</li>
            <li>El sistema debe permitir ofrecer plantillas personalizables para reportes de sesiones.</li>
            <li>El sistema debe permitir generar y almacenar reportes de evaluación psicológica.</li>
            <li>El sistema debe permitir gestionar la historia clínica del paciente según las guías establecidas.</li>
            <li>El sistema debe permitir la carga de documentos en diferentes formatos (PDF, imágenes escaneadas).</li>
            <li>El sistema debe permitir la gestión de la finalización de casos y marcar expedientes como cerrados.</li>
            <li>El sistema debe permitir mantener los expedientes almacenados por 5 años antes de su eliminación.</li>
            <li>El sistema debe permitir notificar a los terapeutas sobre documentos pendientes de entrega.</li>
            <li>El sistema debe permitir la comunicación entre secretaría y terapeutas para validaciones.</li>
            <li>El sistema debe permitir registrar cambios en la asignación de terapeutas en casos de transferencia.</li>
            <li>El sistema debe permitir la digitalización de documentos físicos mediante escaneo.</li>
            <li>El sistema debe permitir la carga y asociación de imágenes de pruebas psicológicas (dibujos, protocolos).</li>
            <li>El sistema debe permitir la integración de herramientas de procesamiento de texto para la redacción de reportes.</li>
            <li>El sistema debe permitir mantener una base de datos de motivos de consulta para estadísticas.</li>
        </ul>
        <h2>Requerimientos No Funcionales Relacionados con IHC</h2>
        <h3>Usabilidad</h3>
        <ul>
            <li>La interfaz debe seguir principios de diseño centrado en el usuario, asegurando que terapeutas, administrativos y coordinadores puedan navegar sin dificultades.</li>
            <li>Se deben reducir los pasos necesarios para realizar tareas críticas, como la consulta y actualización de expedientes, para minimizar la carga administrativa. </li>
            <li>La interfaz debe contar con un sistema de ayuda o tutorial interactivo para nuevos usuarios. </li>
            <li>Se deben utilizar elementos visuales claros y bien organizados, con una jerarquía de información comprensible</li>
        </ul>
        <h3>Seguridad</h3>
        <ul>
            <li>El sistema debe implementar cifrado en la base de datos y en la transmisión de datos para proteger la información de los pacientes contra accesos no autorizados.</li>
            <li>Se debe aplicar control de acceso basado en roles (RBAC), asegurando que cada usuario solo pueda acceder a la información necesaria según su función.</li>
            <li>El sistema debe cumplir con normativas éticas y legales de confidencialidad, como la Ley General de Protección de Datos Personales en Posesión de Sujetos Obligados (LGPDPPSO) y estándares internacionales.</li>
            <li>Las sesiones de usuario deben expirar automáticamente tras un período de inactividad para evitar accesos indebidos.</li>
        </ul>
        <h3>Rendimiento</h3>
        <ul>
            <li>El sistema debe ser capaz de gestionar múltiples consultas simultáneamente sin degradar la experiencia del usuario, optimizando la ejecución de consultas a la base de datos.</li>
            <li>El tiempo de respuesta en la carga y consulta de expedientes no debe exceder los 2 segundos en condiciones normales de operación.</li>
            <li>El sistema debe soportar el acceso concurrente de múltiples usuarios sin afectar la velocidad de procesamiento.</li>
            <li>Se debe utilizar una arquitectura escalable que permita aumentar la capacidad de procesamiento según la demanda.</li>
        </ul>
        <h3>Portabilidad</h3>
        <ul>
            <li>El sistema debe ser accesible desde dispositivos móviles y computadoras, asegurando una experiencia fluida en diferentes resoluciones de pantalla.</li>
            <li>Debe ser compatible con múltiples navegadores web, asegurando una experiencia fluida en diferentes resoluciones de pantalla.</li>
            <li>El diseño debe ser responsivo, adaptándose automáticamente a pantallas de distintos tamaños sin comprometer la usabilidad.</li>
        </ul>
        <h3>Mantenibilidad</h3>
        <ul>
            <li>El sistema debe contar con un proceso sencillo de digitalización de documentos físicos, permitiendo la integración con escáneres y el reconocimiento óptico de caracteres (OCR).</li>
            <li>El código debe estar bien documentado y seguir estándares de desarrollo que faciliten futuras modificaciones o ampliaciones del sistema.</li>
            <li>Se debe permitir la incorporación de nuevos módulos sin afectar el rendimiento ni la estabilidad del sistema.</li>
        </ul>
        <h3>Confiabilidad</h3>
        <ul>
            <li> El sistema debe estar disponible al menos el 99.9% del tiempo en horarios de uso frecuente para garantizar la continuidad del servicio.</li>
            <li>Se deben implementar mecanismos de recuperación ante fallos para evitar la pérdida de información en caso de errores del sistema.</li>
        </ul>
    </body>
</html>
