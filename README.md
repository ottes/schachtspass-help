# Schachtspß Hilfe

Zu finden unter https://help.mine.ottes.club

## Verbindung und Mod-Paket

Das aktuelle ModPaket werde ich hier auch bald verlinken/hinterlegen. Derzeit sollte der Schachtspaßserver schon in der Liste vorhanden sein, falls nicht, lautet die Adresse **minecraft.ottes.club**

## Google-Maps-Style Karte (DynMap)

Zu finden unter https://mine.ottes.club, auch aufzufinden durch Tippen von `/dynmap url` in den Minecraft-Chat.

### Chat

Um den Chat vom Browser aus nutzen zu können, brauchst du zuerst einen Account für die Karte. Das geht, indem du im Spiel einfach `/dynmap webregister` tippst und den Anweisungen folgst.

### Commands

Hier sind alle DynMap Commands im Original auf Englisch, nutzt ChatGPT.

https://github.com/webbukkit/dynmap/wiki/Commands

### Markierungen

Die Karte statet erstmal immer in [Berlin](<[https://foo](https://mine.ottes.club/#Schachtspa%C3%9F;flat;-2899,64,-8328;4)>), im Menü rechts findet man dann "Marker". Einerseits alle Spieler, die gerade online sind, aber auch alle Schilder, die nach der Anleitunge unten erstellt wurden.

Willst du einen Link "teilen", also die aktuelle Ansicht weitergeben, klicke einmal auf das "Kettensymbol" unten links, danach kannst Du den Text in der Browserzeile kopieren/teilen.

Todo: [Markergruppen](https://github.com/webbukkit/dynmap/wiki/Using-Markers#marker-sets) erklären?

#### HowTo Schilder -> Markierungen

Da die [originale Anleitung](https://github.com/webbukkit/dynmap/wiki/Component-Configuration#mc-enablesigns) englisch ist, hier einmal stark vereinfacht und mit Übersicht über die Icons.

Der Spieler kann einen Marker erstellen, indem er ein Schild mit `[dynmap]` in der ersten Zeile aufstellt.

- Die Beschriftung des Markers wird aus der ersten Zeile nach `[dynmap]` genommen, die nicht leer ist

- Das Symbol des Markers kann man ändern, wenn eine Zeile `icon:...` enthält

- Der Marker wird in der Standard-Markergruppe 'Markers' sein, außer eine Zeile enthält `set:...`, um eine andere Gruppe zu wählen

- Nachdem das Schild gespeicher wurde, wird die Zeile `[dynmap]` und alle Einstellungszeilen leer gemacht, sodass nur noch die Beschriftung und eventuelle andere Zeilen sichtbar sind

- Wenn das Schild zerstört wird, wird auch der dazugehörige Marker gelöscht.

Beispiel

    [dynmap] icon:bed
    Mein Bett
