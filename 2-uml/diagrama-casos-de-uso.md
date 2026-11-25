
# Diagrama de casos de uso

## 1. Descripción

El siguiente diagrama representa las principales interacciones entre el jugador y el sistema del videojuego Heal Your World.

El jugador explora el mundo, recolecta recursos, cultiva semillas, construye campamentos y utiliza mecanismos de purificación para recuperar las zonas contaminadas.

## 2. Diagrama

```mermaid
flowchart LR
    J(["Jugador"])

    subgraph HYW["Heal Your World"]
        UC1(["Explorar zonas"])
        UC2(["Recolectar materiales"])
        UC3(["Recoger basura"])
        UC4(["Esquivar ataques"])
        UC5(["Purificar enemigos"])
        UC6(["Cultivar semillas"])
        UC7(["Fabricar sacos de semillas"])
        UC8(["Construir campamentos"])
        UC9(["Frenar propagación de la maleza"])
        UC10(["Consultar progreso"])
        UC11(["Enfrentar al jefe final"])
        UC12(["Sanar el mundo"])
        UC13(["Avanzar en las ramas de IQ"])
    end

    H(["HIGEA"])

    J --- UC1
    J --- UC2
    J --- UC3
    J --- UC4
    J --- UC5
    J --- UC6
    J --- UC7
    J --- UC8
    J --- UC10
    J --- UC11
    J --- UC13

    UC8 -.->|Protección| UC9
    UC5 -.->|Requiere sacos| UC7
    UC11 -.->|Al purificar el núcleo| UC12

    H --- UC10
```

## 3. Actores

| Actor | Descripción |
|---|---|
| Jugador | Controla al protagonista y realiza las acciones principales del videojuego. |
| HIGEA | Deidad que se comunica mediante la estatua y guía al protagonista. |

## 4. Descripción de los casos de uso

| Caso de uso | Descripción |
|---|---|
| Explorar zonas | Recorrer los diferentes biomas del mundo. |
| Recolectar materiales | Obtener recursos naturales y materiales de enemigos. |
| Recoger basura | Limpiar residuos que pueden provocar contaminación. |
| Esquivar ataques | Evitar los ataques de los enemigos corruptos. |
| Purificar enemigos | Lanzar sacos de semillas al foco de corrupción de los enemigos. |
| Cultivar semillas | Plantar semillas y recoger los brotes para obtener más recursos. |
| Fabricar sacos de semillas | Utilizar semillas y fibra para fabricar herramientas de purificación. |
| Construir campamentos | Crear estructuras que permiten establecer zonas de protección. |
| Frenar propagación de la maleza | Los campamentos protegen su radio de influencia. |
| Consultar progreso | Conocer el estado del mundo mediante la guía de HIGEA. |
| Enfrentar al jefe final | Combatir contra el brujo corrupto en la zona final. |
| Sanar el mundo | Purificar el núcleo para alcanzar el desenlace positivo. |
| Avanzar en las ramas de IQ | Mejorar las habilidades de cultivo, construcción, purificación y exploración. |

---

**Proyecto:** Heal Your World  
**Autores:** Geogan Alexander Velazquez Garcia y Alejandro Elías Moreno
