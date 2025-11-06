# 🧩 Comparativo de servicios AWS: EC2 vs Lambda vs Beanstalk

Este documento resume las principales diferencias entre **Amazon EC2**, **AWS Lambda** y **AWS Elastic Beanstalk**, para entender **cuándo y por qué usar cada uno**.

---

## 🧠 Cuadro comparativo

| **Criterio** | **Amazon EC2 (Elastic Compute Cloud)** | **AWS Lambda** | **AWS Elastic Beanstalk** |
|---------------|-----------------------------------------|----------------|----------------------------|
| **Tipo de servicio** | Infraestructura como Servicio (IaaS) | Función como Servicio (FaaS / Serverless) | Plataforma como Servicio (PaaS) |
| **Descripción** | Permite crear y administrar máquinas virtuales configurables (instancias) en la nube. | Ejecuta código sin administrar servidores. | Automatiza el despliegue y escalado de aplicaciones web. |
| **Gestión del servidor** | Totalmente manual (el usuario configura el sistema). | Sin servidor (AWS lo gestiona). | Parcialmente gestionado (AWS maneja la infraestructura). |
| **Modelo de cobro** | Por tiempo de ejecución (hora o segundo). | Por número de ejecuciones y tiempo de cómputo. | Por los recursos que use (EC2, S3, RDS, etc.). |
| **Costo estimado** | Alto si está encendido todo el tiempo. | Bajo para cargas pequeñas o esporádicas. | Variable, según recursos usados. |
| **Escalabilidad** | Manual o automática con Auto Scaling. | Automática por evento (se ejecuta por solicitud). | Automática integrada. |
| **Casos de uso** | Aplicaciones personalizadas, servidores backend, bases de datos, entornos de desarrollo. | Procesamiento de eventos, automatización, APIs sin servidor. | Aplicaciones web listas para producción (Node.js, Python, Java, etc.). |
| **Ventajas** | Control total, alta flexibilidad, integración completa con AWS. | Escalabilidad inmediata, sin mantenimiento, pago exacto por uso. | Despliegue rápido, escalado automático, fácil de usar. |
| **Desventajas** | Más complejo de administrar, riesgo de sobrecostos. | Limitado a funciones cortas (máx. 15 min), no para procesos largos. | Menor control sobre la infraestructura. |
| **Facilidad de uso** | Difícil (nivel avanzado). | Muy fácil (subes tu código y listo). | Intermedio. |
| **Lenguajes soportados** | Cualquiera (depende del SO). | Node.js, Python, Java, Go, .NET, Ruby, etc. | Node.js, Python, Java, .NET, PHP, Go, Ruby. |
| **Fortalezas** | Control y flexibilidad total. | Escalabilidad automática y bajo costo. | Automatización completa del despliegue. |
| **Debilidades** | Requiere mantenimiento constante. | Limitado en tiempo y complejidad. | Menos personalizable. |

---

| **Escenario** | **Servicio recomendado** |
|----------------|--------------------------|
| Necesito control total y personalización | 🖥️ **EC2** |
| Quiero ejecutar código sin manejar servidores | ⚡ **Lambda** |
| Quiero desplegar una app web fácilmente | 🚀 **Beanstalk** |
| Carga continua y predecible | 🖥️ **EC2** |
| Carga intermitente basada en eventos | ⚡ **Lambda** |
| Soy desarrollador y no quiero lidiar con infraestructura | 🚀 **Beanstalk** |

---

### 🏁 Conclusión
- **EC2** → Control total, pero más trabajo. 
- **Lambda** → Simplicidad y ahorro para tareas eventuales. 
- **Beanstalk** → Punto medio: automatización sin perder flexibilidad. 

