## Als Erweiterung verwenden

Dieses Repository kann als **Erweiterung** in MakeCode hinzugefügt werden.

* öffne [https://makecode.calliope.cc/](https://makecode.calliope.cc/)
* klicke auf **Neues Projekt**
* klicke auf **Erweiterungen** unter dem Zahnrad-Menü
* nach **https://github.com/mkleinsb/pxt-gatorlog-calliope** suchen und importieren

## Anschluss des Sparkfun gator:log

* verbinde GND mit - am Calliope
* verbinde 3V3 mit + am Calliope
* verbinde RX  mit  P0
* verbinde TX  mit  P1
* verbinde RST mit  P2

* gator:log initialisieren

## Basic usage

```blocks
// initialize gatorlog and write 400 times the lightlevel to a file
gatorLog.begin()
gatorLog.openFile("Lichtstaerke")
for (let index = 0; index < 400; index++) {
    gatorLog.writeLine("LS " + input.lightLevel())
    basic.pause(150)
}
basic.showIcon(IconNames.Yes)
```


#### Metadaten (verwendet für Suche, Rendering)

* for PXT/calliope
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
