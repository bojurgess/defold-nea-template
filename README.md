# Franklin NEA Template

This template is pre-configured for your NEA project. It includes the following
libraries:

- **[defold-orthographic](https://github.com/britzl/defold-orthographic)** —
  extends Defold's camera system with coordinate projection and camera follow
  utilities. Useful for any game where the viewport needs to move (platformers,
  top-down games, racing games). If your game fits on a single screen, you may
  not need this at all.
- **[defold-event](https://github.com/astrochili/defold-event)** — a simple
  event/messaging system for decoupling game systems from each other.
- **[druid](https://github.com/Insality/druid)** — a UI component library for
  building menus, HUDs, and interactive interfaces.

## Project structure

- `/assets/atlas`: .atlas files (compiled sprite sheets)
- `/assets/audio`: sound effects and music
- `/assets/fonts`: .font files
- `/assets/sprites`: raw source images
- `/assets/tilemaps`: .tilesource and .tilemap files
- `/data`: intended for lua modules that store data (e.g. settings, stats)
- `/events`: defold-event definitions; one module per event type
- `/gui`: .gui and .gui_script files
- `/input`: .input_binding files
- `/levels`: .collection files for each screen or level
- `/objects`: .go game object files
- `/objects/shared`: factories, collision shapes, or other components reused
  across multiple game objects
- `/scripts/behaviours`: .script files that attach to game objects
- `/scripts/modules`: pure Lua modules (no go.* or msg.* calls); data
  definitions, utilities, settings

## Where to start

1. Open [`game.project`](defold://open?path=/game.project) and set your project
   title and resolution.
2. Open [`main.collection`](defold://open?path=/main.collection) - this is your
   bootstrap. You should do your collection proxy loading in here.
3. Put your first level or screen collection in `/levels`.

## Design decisions start here

The template gives you structure and libraries - the rest is up to you. The
choices you make from this point (how you structure your game objects, how
systems communicate, how you manage state) are what your NEA is assessed on.
Keep notes on decisions you make and problems you solve as you go.

## Resources

- [Defold documentation](https://defold.com/learn)
- [Defold forum](https://forum.defold.com)
- [defold-orthographic docs](https://github.com/britzl/defold-orthographic)
- [defold-event docs](https://github.com/astrochili/defold-event)
- [druid docs](https://github.com/Insality/druid)
