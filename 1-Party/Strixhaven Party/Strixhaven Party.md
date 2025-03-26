```meta-bind-button
label: Add Party Member
icon: Player
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: ""
hidden: false
actions:
  - type: templaterCreateNote
    templateFile: z_Templates/TemplatePlayer.md
    folderPath: 1-Party/Strixhaven Party/
    fileName: "[[name]]"
    openNote: true
    openIfAlreadyExists: false

```
```dataview
TABLE WITHOUT ID link(file.name) AS "Character Name", Player, Class, Race, level, Role
from "1-Party/Strixhaven Party"
where (Role = "Player") 
where (Status = "Active") 
```

<br>

```dataview
TABLE WITHOUT ID link(file.name) AS "Character Name", Player, hp, ac, modifier, pasperc As "Passive Perception (WIS)"
from "1-Party"
where (Role = "Player") 
where (Status = "Active") 
```

