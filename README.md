# Django Tutorial 🚀

Este repositorio contiene mi práctica con Django siguiendo el tutorial oficial (en base a la documentación de Django).

---

## 🧭 Índice

- [📌 Estructura del proyecto](#estructura-del-proyecto)
- [✅ Avances personales](#avances-personales)
- [🧠 Apuntes importantes](#apuntes-importantes)
- [🧩 Patrones de Diseño en Django](#patrones-de-diseño-en-django)
- [📂 Documentación extendida](#documentación-extendida)

---

## 📌 Estructura del proyecto

- `mysite/`: configuración principal del proyecto
- `polls/`: primera app del proyecto (encuestas)

---

## ✅ Avances personales

- [x] Crear entorno virtual
- [x] Crear proyecto y app
- [x] Entender la diferencia entre proyecto y app
- [ ] Conectar URLs
- [ ] Templates
- [ ] Modelos y migraciones

---

## 🧠 Apuntes importantes

<details>
<summary>📂 Bases de Datos</summary>

- Django puede trabajar con varias bases de datos. Al usar estas bases, también estamos aplicando el concepto de polimorfismo (POO).
- Bases soportadas: PostgreSQL, MariaDB, MySQL, Oracle y SQLite (esta última viene por defecto).
</details>

<details>
<summary>📌 ¿Qué es un proyecto y una app en Django?</summary>

- **Proyecto**: contenedor de configuración general.
- **App**: funcionalidad específica (como un módulo reutilizable).
</details>

<details>
<summary>💻 Comandos útiles</summary>

### Activar entorno virtual

```bash
source venv/Scripts/activate  # en Git Bash
```

### Crear una nueva app en Django

```bash
python manage.py startapp polls  # polls puede ser cualquier nombre
```

### Comando de Migraciones

```bash
python manage.py migrate  # Ejecuta migraciones para apps en INSTALLED_APPS
```

</details>

---

## 🧩 Patrones de Diseño en Django

<details open>
<summary>📐 MVT (Model - View - Template)</summary>

- **Model**: define la estructura de los datos (`models.py`)
- **View**: maneja la lógica del negocio y respuesta (`views.py`)
- **Template**: define cómo se muestra la información (`templates/`)

> Es el patrón base de Django. Similar a MVC, pero Django se encarga del “Controller” internamente.

</details>

<details>
<summary>🔧 Otros patrones que Django aplica</summary>

| Patrón              | Descripción breve                                       | Ejemplo en Django                        |
| ------------------- | ------------------------------------------------------- | ---------------------------------------- |
| **Singleton**       | Solo se instancia una vez.                              | `settings.py` (configuración global)     |
| **Factory**         | Crea objetos según lógica definida.                     | Creación de vistas, formularios, modelos |
| **Template Method** | Clase base con pasos personalizables.                   | `Class-based views` (`ListView`, etc.)   |
| **Observer**        | Reacciona automáticamente a eventos.                    | `signals.py` (`post_save`, `pre_delete`) |
| **Decorator**       | Añade comportamiento sin modificar la función original. | `@login_required`, `@csrf_exempt`        |

</details>

✅ **Recordatorio:**  
No tengo que implementarlos desde cero. Ya están en uso, y debo:

- Identificarlos en el código
- Aprovecharlos para organizar mejor mis proyectos
- Personalizarlos cuando sea necesario

---

## 📂 Documentación extendida

👉 [Ver apuntes completos](docs/apuntes.md) _(puedes crear este archivo si tu README crece demasiado)_  
👉 [Ver buenas prácticas](docs/buenas-practicas.md)
