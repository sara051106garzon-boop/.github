# Cómo contribuir

Gracias por tomarte el tiempo de mejorar este proyecto. Estas reglas aplican a
todos mis repositorios.

## 1. Antes de empezar

- Revisa si ya existe un **issue** con el mismo tema.
- Si vas a agregar algo grande, abre primero un issue para acordarlo.

## 2. Ramas

Nunca se trabaja directamente sobre `main`.

```bash
git checkout -b nombre_DEV        # rama personal
git checkout -b feat/mi-cambio    # rama por funcionalidad
```

| Tipo de rama | Cuándo usarla |
| :--- | :--- |
| `nombre_DEV` | Trabajo continuo de un integrante del equipo |
| `feat/...` | Una funcionalidad nueva |
| `fix/...` | Corrección de un error |
| `docs/...` | Solo documentación |

## 3. Commits

Se usa [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: agrega validación de placas duplicadas
fix: corrige expiración del token JWT
docs: actualiza la referencia de la API
test: agrega prueba de reserva de celda
chore: actualiza dependencias
```

- En **imperativo** y en **minúscula** después de los dos puntos.
- Un commit = un cambio con sentido propio.

## 4. Pruebas

Antes de subir, la suite completa debe pasar:

```bash
pytest
```

Si el repositorio tiene integración continua, el Pull Request queda bloqueado
hasta que el check esté en verde.

## 5. Pull Request

1. Sube tu rama: `git push origin mi-rama`
2. Abre el PR contra `main` y completa la plantilla.
3. Espera a que pasen las pruebas.
4. Squash and merge (un commit limpio por funcionalidad).

## 6. Estilo de código

- **Python**: PEP 8, nombres en `snake_case`, funciones con docstring.
- **Dart/Flutter**: `flutter analyze` sin advertencias, widgets en `PascalCase`.
- **SQL**: palabras clave en mayúscula, nombres de tabla en plural.
