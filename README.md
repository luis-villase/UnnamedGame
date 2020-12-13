# UnnamedGame

Not much to say yet.

Game for the 2020 Epic Game Jam

##Programs:

* Unreal Engine 4.25
* GIT: https://desktop.github.com/
* Blender: https://www.blender.org/download/

## References and resources:

* Tutorial followed: https://www.youtube.com/watch?v=hRO82u1phyw&list=PLfQ3pODBwOcaV1TdnqNWLTJ4wiUzEvXis
  * E01 = Know the project scope
  * E02 = Download Resources: https://github.com/feureau/BP-3rd-Person-Game/blob/master/ThirdPerson_FBX.zip?raw=true
  * E03 - Import and Skeletons Mesh:
    * Always use the same skeletons assets.
    * Extra joints out of main skeleton is fine, Unreal will keep everything existing as it is; extra stuffs will handle their own.
    * Extra joints inside of main skeleton is bad, it won't know where to place them, and have conflict to identify them.
  * EO4 - Persona Editor, to change Animations
  * E05 - Settings Inputs
  * E06 - Materials: Check more at http://docs.unrealengine.com/latest/INT/Rendering/Materials.html
  * E07 - Blend Spaces:
    * It's how animations blend or merge each other, like switching from walk, run and sprint
    * Blends can be 1D or 2D, for linear or area values.
    * In areas you can mix two variables, like speed and direction.
  * E08 - Animation Blueprints
    * Here we start mixing animation logic, what determines what animation.
  * E09 - State Machines
  * E10 - Create State Machines
  * E11 - Feed Variables in Event Graphs
    * A fancy graph to code logic to wire points.
  * E12 - Create Character Blueprints, more at http://docs.unrealengine.com/latest/INT/Engine/Blueprints/index.html
    * Add Components like camera, something to stick camera
  * E13 - Character Keyboard and Mouse.
  * E14 - Game Mode, Testing, set toggle properties and for controllers.
  * E15 - Touch Controllers, Jump and Cammera hoover.
  * E16 - Intro to Animation Montage
    * Montage is to combine animations
    * Play Animations Selectively
    * Fire off Events
  * E17 - Create Animation Montage for Punching and fixing skeleton
  * E18 - Animation Event Graph to set if it is punching
  * E19 - Continue Set Graphic for isPunching
  * E20 - Using Slots
  * E21 - Agregar Física
    * More about particles: https://docs.unrealengine.com/latest/INT/Engine/Rendering/ParticleSystems/index.html
* Isometric-Shooter: https://github.com/luis-villase/Isometric-Shooter
* Trello Dashboards:
  * Brainstorm: https://trello.com/b/aoPbIFLu/lluvia-de-ideas
  * Unreal HackJam: https://trello.com/b/grFKAnio/unreal-4-hackjam-2020-12
* Assets List: https://docs.google.com/spreadsheets/d/1ql7jah7E7hdI2_T-at6oQfeGtCWuN-CbirU33ebzLdU/edit#gid=0
  * Model: https://sketchfab.com/3d-models/gart220-female-viking-29f88c37b399483dbaba79b4650d4752

## UML Diagrams:
* Read Plant UML Diagrams at https://www.planttext.com/ or any PlanUML parser
* Reference for Plant UML 
