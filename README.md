# Queer Atlas

**Cartografía afectiva de biografías queer en Wikipedia.**

Una plataforma web colaborativa para mapear figuras queer históricas, marcar lo que les agradecemos, y descubrir qué biografías faltan en Wikipedia y Wikidata.

**Demo:** https://[seleneyang].github.io/queer-atlas/

---

## ¿De qué se trata?

Wikipedia cubre las vidas queer y trans de forma desigual: muchas figuras que dieron forma a la historia queer no cuentan con un artículo sobre sus vidas o trayectorias, y otras solo existen en un solo idioma. Desde el *Queer Atlas* se busca visibilizar estas ausencias, para colectivizar la memoria, el agradecimiento y el dolor que sentimos por las vidas de estas personas. 

**¿Cómo utilizar este atlas?**

1. Buscás el nombre de alguien que te importa.
2. La herramienta jala sus datos desde Wikidata.
3. La ubicás en el mapa.
4. Marcás **qué le agradecés** — coraje, visibilidad, comunidad, lenguaje, arte, ternura.
5. Marcás **qué te duele** (opcional) — rabia, duelo. 
6. Si Wikipedia no tiene su biografía en español, inglés, francés o portugués, un click te lleva al editor con los datos de Wikidata precargados.

Cada entrada genera una **marca de gratitud**: una firma visual única que combina las ocho dimensiones en un blob de color. La galería las acumula. El mapa coloca pines del color de la dimensión dominante.

---

## Wikiproyecto:LGBT

Construido en diálogo con el [Wikiproyecto:LGBT](https://es.wikipedia.org/wiki/Wikiproyecto:LGBT) de Wikipedia en español. La lista de figuras sugeridas que carga la herramienta se inspira en sus [Eventos del Mes](https://es.wikipedia.org/wiki/Wikiproyecto:LGBT/Evento_del_mes) y solicitudes de la comunidad.

Si te interesa crear o mejorar biografías queer/trans en Wikipedia desde una perspectiva comunitaria, ese es el lugar para sumarte.

---

## Cómo se usa

Tres formas de empezar:

- **Tocá una figura sugerida** en el panel "Inspirado en el Wikiproyecto:LGBT".
- **Buscá por nombre** en el campo de búsqueda — autocompleta contra Wikidata.
- **Explorá la galería** y el mapa para ver lo que ya cargaste (cada navegador tiene su propia galería local por ahora).

No requiere instalación y sirve desde cualquier navegador. 

---

## Tecnología

- HTML/CSS/JS vanilla, single page, todo client-side
- **Wikidata API** (`wbsearchentities`, `wbgetentities`) para búsqueda y datos biográficos
- **Sitelinks** de Wikidata para chequear existencia del artículo por idioma
- **Leaflet** + **Wikimedia Maps** para el mapa
- **LocalStorage** para persistencia local
- Tipografías: **Elms Sans** + **Quicksand** (Google Fonts)

No tiene un backend o dependencias instaladas, solo CDNs. 

---

## Estado actual

Se encuentra en Versión **0.1 — prototipo**. 

Roadmap:

- [ ] **Galería colectiva** vía backend compartido (hoy es individual en cada navegador)
- [ ] **Lectura directa de las listas del Wikiproyecto:LGBT** vía MediaWiki API, en lugar de la semilla curada manualmente
- [ ] **Verificación y expansión** de los Q-IDs sugeridos
- [ ] **Wikidata SPARQL** para encontrar figuras queer no listadas explícitamente
- [ ] **Queer Atlas Watch** — herramienta hermana para monitoreo comunitario de vandalismo en biografías queer y trans, usando la API de Lift Wing

---

## Contribuir

Issues, PRs y comentarios bienvenidos. Si encontrás errores en los Q-IDs de la lista semilla, querés agregar figuras, o tenés ideas sobre los ejes de gratitud y dolor — abrí un issue.

Para discusiones más amplias sobre cómo cerrar brechas de cobertura queer en Wikipedia, el espacio natural es el [Wikiproyecto:LGBT](https://es.wikipedia.org/wiki/Wikiproyecto:LGBT).

---

## Licencia

Código bajo licencia [MIT](LICENSE). Forkealo, adaptalo, llevalo a tu comunidad.

---

## Créditos

Construido por **Selene Yang** con miras a presentar en [Queering Wiki 2026](https://meta.wikimedia.org/wiki/Queering_Wiki) (Montréal, 23–25 de octubre de 2026).
