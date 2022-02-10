# I/O

The keyboard and mouse are set up in objects, so you can easily access their info.

> ex: &nbsp; `bob.x = mouse.x + 50;`

### mouse
value | type | example
--- | --- |---
x | int | `alert(mouse.x)`
y | int | `alert(mouse.y)`
moved | func | `mouse.moved = ()=>{ }`
up | func | `mouse.up = ()=>{ }`
down | func | `mouse.down = ()=>{ }`
pressed | func | `if(mouse.pressed){alert()}`
cursor | str | `mouse.cursor = 'red'` ***(use CSS)***
button | int | `mouse.down=()=>{if(button==3){alert()}}`


### Keyboard
value | type | example
--- | --- |---
name | str | `alert(key.name)`
code | int | `alert(key.code)`
up | func | `mouse.up = ()=>{ }`
down | func | `mouse.down = ()=>{ }`
pressed | func | `if(mouse.pressed){alert()}` &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;

### page
value | example
 --- | ---
selectable | `page.selectable = false`
editable | `page.editable = true`
width | `w = page.width`
height | `h = page.height`
loaded | `if(page.loaded){ alert() }`  &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;
