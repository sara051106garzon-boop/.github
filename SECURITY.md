# Política de seguridad

## Versiones soportadas

| Versión | Soporte |
| :--- | :--- |
| `1.x` | ✅ Recibe correcciones |
| `< 1.0` | ❌ Sin soporte |

## Cómo reportar una vulnerabilidad

**No abras un issue público.** Escribe a:

- **Correo:** *(agrega aquí tu correo de contacto)*
- **Asunto:** `[SEGURIDAD] <repositorio> — descripción breve`

Incluye:

1. El repositorio y la versión afectada.
2. Los pasos para reproducir el problema.
3. El impacto que crees que tiene.
4. Una posible solución, si la conoces.

## Qué puedes esperar

| Plazo | Acción |
| :--- | :--- |
| 72 horas | Confirmación de que recibí el reporte |
| 7 días | Evaluación inicial y plan de corrección |
| 30 días | Corrección publicada, si se confirma la falla |

## Buenas prácticas del proyecto

- Las credenciales **nunca** se suben al repositorio; van en `.env`, que está en `.gitignore`.
- Los tokens JWT tienen expiración y se validan en el servidor.
- Las contraseñas se guardan con hash, nunca en texto plano.
- Dependabot revisa las dependencias cada semana.
