# Orbis Arcana: El arco bajo el trigal

*English below.*

Aventura inicial para el sistema **Orbis Arcana** en Foundry VTT (v14). Tres actos en Linar, la villa del trigo de
Valtera, para 4 o 5 personajes del nivel 1 al 4. Un contrato del Gremio contra una plaga de lomocristales termina en un
arco antiguo que se encendió fuera de la Conjunción.

Trae, en español y en inglés (un compendio de Aventura por idioma):

- el texto para el DJ: un diario por parte y una página por escena, con los encuentros enlazados a sus actores;
- los PNJ y las criaturas de cada encuentro, en carpetas por acto;
- las escenas con sus mapas, muros, luces y notas;
- las notas de diseño (lo decidido y lo que falta probar en mesa), en un diario aparte (solo para el DJ).

## Instalación

1. Instalar antes el sistema **Orbis Arcana** (versión 0.4.1 o posterior).
2. En la pantalla de configuración de Foundry, *Complementos* → *Instalar módulo* → pegar en *URL del manifiesto*:
   `https://github.com/mvolgyi/orbis-arcana-valtera/releases/latest/download/module.json`
3. Hay dos formas de jugarla:
   - **Mundo nuevo listo para jugar:** al crear un mundo con el sistema Orbis Arcana, Foundry ofrece armarlo con la
     aventura (en español).
   - **En un mundo propio:** activar el módulo, abrir el compendio *El arco bajo el trigal* (o *The Arch Under the
     Wheat*) y elegir *Importar aventura*.

---

# Orbis Arcana: The Arch Under the Wheat

Starting adventure for the **Orbis Arcana** system on Foundry VTT (v14). Three acts in Linar, Valtera's wheat village,
for 4 or 5 characters from level 1 to 4. A Guild contract against a plague of shardbacks ends at an ancient arch that
lit up outside the Conjunction.

It includes, in Spanish and English (one Adventure compendium per language):

- the GM text: one journal entry per part and one page per scene, with encounters linked to their actors;
- the NPCs and the creatures of every encounter, in one folder per act;
- the scenes with their maps, walls, lights, and notes;
- the design notes (what was decided and what still needs playtesting), in a separate journal entry (GM only).

## Installation

1. First install the **Orbis Arcana** system (version 0.4.1 or later).
2. In Foundry's setup screen, *Add-on Modules* → *Install Module* → paste into *Manifest URL*:
   `https://github.com/mvolgyi/orbis-arcana-valtera/releases/latest/download/module.json`
3. There are two ways to play it:
   - **New ready-to-play world:** when you create a world with the Orbis Arcana system, Foundry offers to build it with
     the adventure (in Spanish).
   - **In your own world:** enable the module, open the *The Arch Under the Wheat* compendium (or *El arco bajo el
     trigal*) and choose *Import Adventure*.

## Para desarrollar / Development

Las fuentes están en `datos/` (texto en `datos/aventura/es.md` y `en.md`, PNJ en `datos/pnj.mjs`, escenas en
`datos/escenas/*.json`). Los compendios se arman desde la raíz del repositorio del sistema:

```bash
tools/node.sh tools/modulo-valtera.mjs        # arma packs/aventura-es y packs/adventure-en
tools/node.sh tools/test-modulo-valtera.mjs   # pruebas
tools/node.sh tools/empaquetar-valtera.mjs    # dist/orbis-arcana-valtera-<versión>.zip y dist/module.json
```
