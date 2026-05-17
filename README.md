<div align="center">
  <img src="https://github.com/nandocdev/nandocdev/blob/main/assets/banner-github.png" width="800"/>
</div>

# Fernando Castillo

Backend Engineer enfocado en sistemas reales.  
Laravel + PostgreSQL + Node.js.

Diseño **monolitos modulares mantenibles** y evito complejidad innecesaria.

---

## Contacto

- LinkedIn: https://linkedin.com/in/fernando-castillo-vald%C3%A9s-38458aa1  
- X: https://x.com/nandocdev  
- Email: nandocdev@gmail.com  

---

## Stack

**Backend**
- Laravel / PHP
- Node.js (TypeScript)
- Python (automatización)

**Data**
- PostgreSQL (principal)
- MySQL
- MongoDB (casos específicos)

**Frontend**
- Livewire / Blade
- Vue (cuando aplica)

**Infra**
- Docker
- CI/CD básico (GitHub Actions)

---

## Enfoque

- Monolito modular > microservicios prematuros  
- Optimizar después de medir  
- Código entendible a las 3 a.m.  
- Evitar abstracciones innecesarias  

---

## Proyectos

### ReservEase — SaaS de reservas

**Problema:** pequeños negocios sin sistema de agenda estructurado  

**Solución:**
- Multi-tenant en Laravel
- Agenda visual con control por negocio
- Configuración dinámica

**Decisiones**
- Monolito modular → menor complejidad operativa
- MySQL → suficiente para carga actual

**Trade-offs**
- Escalabilidad limitada sin partición futura
- Falta de cacheo en consultas pesadas

**Riesgos**
- N+1 en agenda si crece volumen
- Necesidad de colas para notificaciones

Repo: https://github.com/nandocdev/reservease

---

### WhatsApp Automation — Gestión de conversaciones

**Problema:** manejo manual e ineficiente de chats  

**Solución:**
- Clasificación automática
- Asignación de agentes
- Estados de conversación

**Decisiones**
- Node.js + TypeScript → I/O intensivo
- Arquitectura modular (no microservicios)

**Trade-offs**
- Dependencia de whatsapp-web.js (inestable)
- Persistencia limitada sin eventos durables

**Riesgos**
- Rate limits / bloqueos
- Pérdida de sesión

Repo: https://github.com/nandocdev/whatsapp-automation

---

## Actualmente

- Construyendo SaaS reales (no demos)
- Mejorando testing y CI/CD
- Migrando parte del stack a C# / .NET

---

## Regla personal

> Si no puedo explicarlo simple, está mal diseñado.
