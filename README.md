# <b>Creación de canalizaciones CI/CD independientes con GitHub Actions</b> <br/> Mono-repositorio, Multi-repositorio y Meta-repositorio

## Mono-repositorio

El Mono-repositorio ( _mono-repo_) es un concepto de arquitectura y una estrategia de gestión del código fuente que consiste en agrupar en un único contenedor de código todos los componentes de la solución. Un Mono-repositorio en lugar de administrar múltiples repositorios, mantiene todas sus partes de código aisladas dentro de un único espacio aunque están virtualmente separadas siguiendo alguna convención definida por el equipo de trabajo. Pero el concepto de aislamiento aquí no debe confundirse, un mono-repositorio es una estrategia de gestión y no implica crear [aplicaciones monolíticas](https://es.wikipedia.org/wiki/Aplicaci%C3%B3n_monol%C3%ADtica). Generalmente es todo lo contrario, el concepto mantiene la correcta separación de dependencias que las arquitecturas de [micro-servicios](https://es.wikipedia.org/wiki/Arquitectura_de_microservicios) requieren y su uso no compromete otros principios de desarrollo. Una característica importante para un mono-repo es que, si bien contiene múltiples proyectos distintos, estos deben tener entre ellos relaciones bien definidas. El mono-repo no se trata de colocar el código en un solo repositorio, si no hay relaciones bien definidas entre los proyecto, no se denomina mono-repo.

## Multi-repositorio

El enfoque multi-repositorio, como su nombre lo indica, utiliza varios repositorios para albergar los múltiples componentes, librerías o servicios de un proyecto desarrollado por una empresa. En su forma más extrema, alojará cada conjunto mínimo de código utilizable o cada funcionalidad independiente (como un micro-servicio) en un repositorio individual.

## Meta-repositorio

Los meta-repos combinan la comodidad de un mono-repo con la flexibilidad de los repositorios de código separados. Pero aún así, tener repositorios de código separados añade complejidad, y sería mejor si pudiéramos ceñirnos al mono-repo más simple durante el mayor tiempo posible.

Hay otras razones para dividir el mono-repo. Para una empresa en crecimiento, la división a repositorios separados puede permitirle escalar a través de un equipo de desarrollo en crecimiento.

Pero si lo que desea es separar las tuberías de CD, ¿no sería bueno poder seguir con el mono-repo más simple durante más tiempo y ser capaz de tener tuberías de CD separadas para cada sub-proyecto?

Bueno, la buena noticia es que es posible. Puedes tener múltiples CD pipelines - al menos puedes usar GitHub Actions - lo que nos permite mantener la simplicidad de nuestro mono-repo durante mucho más tiempo.

### Bibliografía

- Ashley, D (2022) _Creating separate monorepo CI/CD pipelines with GitHub Actions_ LogRocker. Recuperado de: https://blog.logrocket.com/creating-separate-monorepo-ci-cd-pipelines-github-actions/

- Ramirez, I. (2022) _Desarrollo de aplicaciones con arquitectura mono-repositorio_. GitHub. Recuperado de: https://github.com/Igvir
