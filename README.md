# Biblioteca técnica

Documentación de estudio sobre mis proyectos de software. Es HTML y CSS estático: abre `index.html` en un navegador y listo, sin servidor ni dependencias.

## Estructura

```
index.html          catálogo general
styles.css          estilos del catálogo
proyectos/
  <proyecto>/
    index.html      documento del proyecto
    styles.css      estilos propios de ese documento
```

Cada documento es independiente: su propio CSS y enlaces relativos. El único JavaScript abre las secciones plegables antes de imprimir, para que el PDF las incluya.

## Convenciones

- **Etiquetas de evidencia**: Verificado, Configurado (sin uso confirmado), Documentado, Inferido, Pendiente, No encontrado.
- **Referencias al código**: rutas relativas a la raíz del repositorio analizado, con rangos de líneas válidos para el commit indicado en la cabecera de cada documento.
- **Fragmentos**: breves y copiados del repo; cualquier ejemplo que no esté en el repo se marca como «ejemplo didáctico».
- **Sin secretos**: nunca se copian valores de `.env`, tokens ni credenciales; solo los nombres de las variables.

## Mantenimiento

1. Cuando un proyecto cambie de forma importante, vuelve a analizarlo y actualiza el commit y la fecha en la cabecera.
2. Comprueba que las rutas citadas existan: `git cat-file -e <commit>:<ruta>`.
3. Valida el HTML (por ejemplo con `npx html-validate`) y revisa los enlaces internos.

## Estado

| Proyecto | Estado |
| --- | --- |
| Vectra | Documentado (piloto) · `b4caeb5` · 2026-10-14 |
| Vigía, WikiToon, MediReserva, Portafolio, WhatsApp_IA, Auditoria_AEO, AI OS, Job Tracker, Mister Barber, base360-design-challenge | Pendientes |
