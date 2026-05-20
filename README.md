# Simulador de Planificación de CPU

Herramienta interactiva para visualizar y entender algoritmos de planificación de procesos en sistemas operativos.

## 👤 Autor

**Manuel Alonso Carracedo**
- Email: manuel.alonso.carracedo@uvigo.gal
- ResearchGate: [Perfil](https://www.researchgate.net/profile/Manuel-Alonso-Carracedo)
- ORCID: [0009-0001-5037-5826](https://orcid.org/0009-0001-5037-5826)

## ✨ Características

- **Simulación paso a paso**: Play/Pausa, retroceso, control de velocidad
- **Diagrama de Gantt**: Visualización de ejecución de procesos
- **Métricas en tiempo real**: Tiempos de espera, retorno y respuesta
- **Configuración flexible**: Tabla editable de procesos, ejemplos precargados
- **Detección de inanición**: Identifica cuando procesos sufren espera prolongada
- **Atajos de teclado**: Espacio (play), flechas (paso), R (reset)

## 🔄 Algoritmos Soportados

| Algoritmo | Tipo | Características |
|-----------|------|-----------------|
| **FCFS** | No preemptivo | Orden de llegada |
| **SJF** | No preemptivo | Ráfaga más corta |
| **SRTF** | Preemptivo | Tiempo restante mínimo |
| **Round Robin** | Preemptivo | Quantum fijo |
| **Multinivel** | Preemptivo | 3 colas por prioridad |

## 🚀 Uso

1. Selecciona un algoritmo
2. Configura procesos (PID, llegada, ráfaga)
3. Ajusta parámetros (quantum para RR)
4. Simula con ▶ o avanza paso a paso con ⏭

## 🛠️ Tecnologías

- HTML5 + CSS3 + Vanilla JavaScript
- Sin dependencias externas
- Responsive design

## 📖 Más Información

Herramienta diseñada para visualizar:
- Diferencias entre algoritmos apropiativos y no apropiativos
- Concepto de inanición (*starvation*)
- Efecto convoy en FCFS
- Impacto del quantum en Round Robin
- Planificación multinivel con prioridades

---

**Versión 1.0**
