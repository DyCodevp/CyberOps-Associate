# ** CyberOps Associate v1.0 **

# 1 Modulo

# slide 1

## Título del módulo: El peligro

> ### **Secuestro de personas**

Los hackers crean una red
wifi para suplantar otra
produciendo que las personas
se conecten y los hackers
tengan acceso a sus datos.

# slide 2

> ### **Empresas a las que se le solicitan rescates**

Normalmente estas empresas
son grandes y pueden ser atacadas
con la minima vulnerabilidad
como un documento, un correo malicioso
con un ransomware y este ocacione
que su activo mas importante se vean
comprometidos.El objetivo de estos
rescates es ganar dinero.

# slide 3

> ### **Naciones objetivo**

La mayoria de programas de malware son
tan sofisticados y costosos de crear
que solamente las grandes empresas o
naciones pueden tener la influencia
y financiamiento para crearlos y atacar
la infraestructura o sistemas de una
nacion.

# slide 4

> ### **Agentes de amenazas**

En estos agentes se encuentran los
aficionados, hacktivistas, grupos de
crimen organizado, agentes patrocinados
por el estado y grupos terroristas.

- Aficionados
  - Los **script kiddies** tienes poca habilidad o casi nula
    utilizan herramientas ya existentes o instrucciones que
    buscan en internet para comenzar a tratar de atacar apesar de ser un ataque bastante basico puede llegar a dañar empresas o personas con malas practicas en internet.
- Hactivistas
  - Los **hacktivistas** son hackers ya mas expertos que
    protestan contra las ideas politicas y sociales, estan
    en contra de las organizaciones o los gobiernos, estos
    filtran información confidencial y interrumpen servios web
    con ataque (DDos) que lo que hace es saturar la pagina con
    muchas peticiones.
- Grupo Financiero
  - El mayor interes de estos grupos son obtener acceso a nuestras cuentas bancarias, datos personales, y cualquier
    otro dato que les sirva para conseguir dinero.
- Agentes patrocinados por el estado o comercios
  - Los paises atacan a otros paises o espian para conseguir informacion que les interese y les den ventaja para aprovecharse de esta o dañar al organismo.
    // --- tres lineas es para hacer

---

> ### ¿Es seguro el internet de las cosas?

El internet de las cosas(IoT) esta a nuestro alrededor y crece muy rapidamente, IoT ayuda a las personas a conectar dispositivos
para asi mejorar la calidad de vida.¿Es vulverable a ataques el termoestato inteligente de su hogar?¿Que tan frecuente reciben los parches estos dispositivos? Algunos dispositivos nisiquiera se desarrollaron para recibir actualizaciones.
Estas situaciones son las que aprovechan los delicuentes ciberneticos y crean vulnerabilidad a los dueños de estos dispositivos.
Un ejemplo de ciberataque seria [Ciberataque a Dyn](https://www.incibe-cert.es/blog/ddos-actualidad-iot-y-los-dns-dyn).

> ### PII, PHI y PSI

- PII (personal indentifiable information)
  - Nombre
  - Número de seguridad social
  - Fecha de nacimiento
  - Número de tarjetas de crédito
  - Número de cuentas bancarias
  - identificación emitida por el gobierno
  - información sobre la dirección
    Uno de los objetivos lucrativos de los ciberdelicuentes es vender listas de PII en la deep web.
- PHI (Protected Health information)
  - Es un subconjunto de la PII. La comunidad médica crea y mantiene registros médicos electrónicos (EMR) que contienen PHI.
- PSI (Personal Security information)
  - Es otro tipo de información personal. Esta información incluye nombres de usuario, contraseñas y otra información relacionada con la seguridad que los individuos utilizan para acceder a información o servicios de la red.

### Pérdida de la ventaja competitiva

Las empresas están cada vez más preocupadas por el espionaje corporativo en el ciberespacio. La pérdida de propiedad intelectual de los competidores es motivo de grave preocupación. Una importante preocupación adicional es la pérdida de confianza que surge cuando una empresa es incapaz de proteger los datos personales de sus clientes.

### Política y seguridad nacional

No solo las empresas sufren ataques.un hacker publicó los datos personales de 20 000 empleados de la Oficina Federal de Investigaciones (FBI).

El gusano Stuxnet se diseñó específicamente para impedir el avance de Irán en el enriquecimiento de uranio que podría usarse en un arma nuclear. Stuxnet es un claro ejemplo de un ataque a la red motivado por asuntos de seguridad nacional. La ciberguerra es una posibilidad concreta.

# Modulo 2

> ## Elementos de un SOC
>
> (Security operations center)
> Los roles de trabajo en un SOC están evolucionando rápidamente. Tradicionalmente, los SOC asignan roles de trabajo por niveles, de acuerdo con la experiencia y las responsabilidades que requiere para cada uno

- Analista de alertas 1
  Estos profesionales monitorean las alertas entrantes, verifican que sea un incidente verdadero haya ocurrido y reenvían los tickets al nivel 2, si es necesario
- Respuestas de incedentes 2
  Estos profesionales son responsables de realizar una investigación profunda de los incidentes y aconsejar soluciones o acciones para ser tomadas.
- Cazardor de amenazas de nivel 3
  Estos profesionales tienen un nivel experto de habilidad en la red, punto terminal, inteligencia de amenazas e ingeniería reversa de malware Son especialistas en seguir los procesos del malware para determinar su impacto y cómo eliminarlo.

- Administrador del SOC
  Este profesional administra todos los recursos del SOC y sirve como punto de contacto con el resto de la organización o el cliente

> ##### El sistema de tickets es frecuentemente utilizado para asignar alertas a la cola para que un analista las investigue

> Si el ticket no puede ser resuelto, el analista de ciberseguridad lo reenvía al encargado de respuesta de nivel 2 para una investigación más profunda y una solución.

> Si el encargado de respuesta no puede resolver el ticket, será reenviado al personal de nivel 3 con el conocimiento profundo y habilidades de caza de amenazas.

### Tecnologías en el SOC: SIEM

(Security Information and Event Management System)

SOC necesita un sistema de administración de información y eventos de seguridad para dar sentido a todos los datos que generan los firewalls, dispositivos de red, sistemas de detección de intrusiones y otros dispositivos.

Se utilizan para recopilar y filtrar datos, detectar y clasificar amenazas y analizar e investigar amenazas. Los sistemas SIEM también pueden administrar recursos para implementar medidas preventivas y hacer frente a amenazas futuras.

### Tecnologías en el SOC: SOAR

> La coordinación de seguridad, automatización y respuesta

SOAR son similares a los SIEM en el sentido de que agregan, correlacionan y analizan alertas. Sin embargo, la tecnología SOAR va un paso más allá al integrar la inteligencia de amenazas y automatizar los flujos de trabajo de investigación y respuesta de incidentes basados en playbooks desarrollados por el equipo de seguridad.

##### Plataformas de seguridad SOAR

- Recopilar datos de alarma de cada componente del sistema.
- Proporcionar herramientas que permitan rebuscar, evaluar e investigar casos.
- automatizar flujos de trabajo de respuesta a incidentes complejos que permiten una respuesta más rápida y estrategias de defensa adaptada.
- playbooks predefinidos que permitan la respuesta automática a amenazas específicas

El SOAR procesará muchas de estas alertas automáticamente y permitirá al personal de seguridad centrarse en amenazas más complejos y potencialmente dañinos.

### Métricas SOC

Un SOC es de vital importancia para la seguridad de una organización.

Es importante comprender qué tan bien funciona el SOC para que se puedan realizar mejoras en las personas, los procesos y las tecnologías que componen el SOC.

Métricas o indicadores clave de rendimiento (KPI) para medir diferentes aspectos específicos del rendimiento del SOC.cinco métricas se utilizan comúnmente como métricas SOC.

- Tiempo de permanencia:el tiempo que los actores de amenazas tienen acceso a una red antes de ser detectados y su acceso se detiene.

- Tiempo medio de detección (MTTD):el tiempo medio que tarda el personal de SOC en identificar incidentes de seguridad válidos se han producido en la red.

- Tiempo medio de respuesta (MTTR):el tiempo medio que se tarda en detener y corregir un incidente de seguridad.
- Tiempo medio para contener (MTTC):el tiempo necesario para evitar que el incidente cause más daños a los sistemas o datos.

- Tiempo de control: el tiempo necesario para detener la propagación de malware en la red.

### Seguridad empresarial y administrada

Para redes medianas y grandes, la organización se beneficiará de implementar un SOC de nivel empresarial.

> Cisco cuenta con un equipo de expertos que ayudan a garantizar la resolución oportuna y precisa de incidentes.
>
> - Servicio Cisco Smart Net Total Care para la resolución rápida de problemas
> - Equipo de respuesta ante los incidentes de seguridad de los productos (PSIRT) de Cisco
> - Equipo de respuesta ante los incidentes de seguridad de las computadoras (CSIRT) de Cisco
> - Servicios administrados de Cisco
> - Operaciones tácticas de Cisco (TacOps)
> - Programa de seguridad física y de seguridad de Cisco

### Comparación entre seguridad y disponibilidad

La mayoría de las redes empresariales tienen que estar funcionando en todo momento. El personal de seguridad entiende que, para que la organización logre sus prioridades, debe mantenerse la disponibilidad de la red.

Cada empresa o industria tiene una tolerancia limitada al tiempo de inactividad de la red.Esa tolerancia suele basarse en una comparación entre el costo del tiempo de inactividad y el costo de protección contra el tiempo de inactividad.
El tiempo de actividad preferido a menudo se mide en la cantidad de minutos de inactividad en un año

> “cinco nueves” indica que la red está activa el 99,999 % del tiempo, es decir, permanece inactiva menos de 5 minutos por año. “Cuatro nueves” equivale a un tiempo de inactividad de 53 minutos por año.

| Disponibilidad %           | Tiempo de incatividad |
| -------------------------- | --------------------- |
| 99,8 %                     | 17,52 horas           |
| 99,9% ("tres nueves")      | 8,76 horas            |
| 99,99% ("cuatro nueves")   | 52,56 minutos         |
| 99,999% ("cinco nueves")   | 5,256 minutos         |
| 99,9999% ("seis nueves")   | 31.56 segundos        |
| 99,99999% ("siete nueves") | 3.16 segundos         |

> ##### El nivel de seguridad no debe ser tan alto como para interferir en las necesidades de los empleados o las funciones empresariales.
