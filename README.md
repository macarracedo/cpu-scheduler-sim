# Simulador de Planificación de CPU

Herramienta interactiva y didáctica para visualizar y entender algoritmos de planificación de procesos en sistemas operativos.

## 🚀 Despliegue

La aplicación se encuentra desplegada y lista para su uso en: **[simulador.lia2.org](https://simulador.lia2.org)**

## 👤 Autor

**Manuel Alonso Carracedo**
- Email: manuel.alonso.carracedo@uvigo.gal
- ResearchGate: [Perfil](https://www.researchgate.net/profile/Manuel-Alonso-Carracedo)
- ORCID: [0009-0001-5037-5826](https://orcid.org/0009-0001-5037-5826)

## ✨ Características

### Simulación
- **Play/Pausa, paso a paso y retroceso**: Controles intuitivos
- **Control de velocidad**: 100 ms a 2000 ms por tick
- **Atajos de teclado**: Espacio (play), flechas (paso), R (reset)
- **Reinicio**: Volver al estado inicial

### Visualización
- **Diagrama de Gantt interactivo**: Con scroll y eje de tiempo
- **Estado de colas en tiempo real**: Procesos listos, en ejecución, pendientes
- **Métricas detalladas**: Tiempos de espera, retorno, respuesta por proceso
- **Totales y promedios**: Estadísticas globales

### Configuración
- **Tabla editable de procesos**: Añadir, eliminar, modificar
- **Ejemplos precargados**: Uno por algoritmo optimizado
- **Parámetros ajustables**: Quantum variable para Round Robin
- **Modal "Acerca de"**: Información del autor y contexto académico

### Didáctica de Inanición
- **Botón de caso de inanición**: Carga configuración diseñada para SJF, SJF Apropiativo y SRTF
- **Modal de confirmación**: Antes de sobrescribir procesos
- **Detección automática**: Identifica espera prolongada
- **"¿Qué ha pasado?"**: Botón que explica la inanición ocurrida con análisis específico del algoritmo
- **Banners explicativos**: Eventos relevantes durante simulación

## 🔄 Algoritmos Soportados

| Algoritmo | Tipo | Características |
|-----------|------|-----------------|
| **FCFS** | No preemptivo | Orden de llegada |
| **SJF** | No preemptivo | Ráfaga más corta |
| **SJF Apropiativo** | Preemptivo | Compara ráfaga original |
| **SRTF** | Preemptivo | Tiempo restante mínimo |
| **Round Robin** | Preemptivo | Quantum fijo |
| **Multinivel** | Preemptivo | 3 colas por prioridad (Q0: RR q=2, Q1: RR q=4, Q2: FCFS) |

## 🚀 Uso

1. Selecciona un algoritmo
2. Configura procesos (PID, llegada, ráfaga, cola si es multinivel)
3. Ajusta parámetros (quantum, etc.)
4. **[Opcional]** Carga un caso de inanición para SJF/SJFP/SRTF
5. Simula con ▶ o avanza paso a paso con ⏭
6. Observa explicaciones automáticas en banners
7. Al finalizar un caso de inanición, interpreta el análisis en "¿Qué ha pasado?"

## 🛠️ Tecnologías

- HTML5 + CSS3 (Grid, Flexbox, Animaciones)
- Vanilla JavaScript (sin dependencias)
- Modal infrastructure para About y análisis
- Responsive design

## 📖 Conceptos Pedagógicos

Visualiza y experimenta con:
- Diferencias entre algoritmos apropiativos y no apropiativos
- **Inanición** (*starvation*): Espera indefinida en SJF, SJFP y multinivel
- Efecto convoy en FCFS
- Impacto del quantum en Round Robin
- Planificación multinivel con preemption entre colas
- Diferencia entre comparar ráfaga vs. tiempo restante

## 📝 Versión

**Versión 2.0**

Mejoras respecto a v1:
- ✅ Algoritmo SJF Apropiativo (SJFP)
- ✅ Modal "Acerca de" con datos del autor
- ✅ Casos de inanición precargados con análisis detallado
- ✅ Botón "¿Qué ha pasado?" para explicar inanición
- ✅ Métricas ampliadas: totales + promedios
- ✅ Mejor etiquetado de campos en multinivel
