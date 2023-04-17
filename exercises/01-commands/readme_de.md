# PowerShell Befehle

PowerShell Befehle werden **Cmdlets** bezeichnet.

Reine PowerShell Cmdlets haben den Aufbau **Verb-Substantiv**. Befehle die diesem Aufbau nicht folgen sind entweder ältere Cmd-Befehle (wie `ping`), Befehle andere Terminals (z.B. bash Befehl `ls`) oder Aliase von Cmdlets.

## Aliase

Die meisten Cmdlets besitzt ein oder mehrere Alias um die Eingabe zu vereinfachen. So kann z.B. für `Get-ChildItem` auch einfach nur `gci` oder `dir` eingegeben werden.

Zu welchen Cmdlet ein Alias gehört kann mittels `Get-Alias` herausgefunden werden.

`Get-Alias <Alias>` z.B. `Get-Alias dir`

Andersherum, welche Aliase ein Cmdlet besitzt ebenfalls mit `Get-Alias` unter Verwendung des Parameters `-Definition`.

`Get-Alias -Definition <Cmdlet>` z.B. `Get-Alias -Definition Get-ChildItem`

---
Es ist auch möglich eigene Alias für vorhandene Cmdlet zu erstellen. Es können jedoch KEINE Alias für komplette Cmdlet mit Parameter erstellt werden!

Hierfür gibt es 2 Cmdlets:

`New-Alias` : Zum erstellen eines **neuen** Aliases. Sollte dieser bereits existieren, gibt es einen Fehler.<br />
`Set-Alias` : Zum erstellen **oder** ändern eines Aliases. Hier werden bereits vorhandene Aliase überschrieben.

Beide haben die Möglichkeiten Beschreibungen, Optionen, Scopes und andere Parameter für den Alias zu erstellen. Der einfache Syntax ist jedoch: `New-Alias <AliasName> <CmdletName>` (für `Set-Alias` der Gleiche).

z.B. `New-Alias Inhalt Get-ChildItems`

Es können auch Aliase auf Aliase erstellt werden: `New-Alias Inhalt gci`

---
Alias entfernen kann man mit `Remove-Alias` wobei das nur selten gebraucht wird.

Die erstellten Aliase sind **NUR** in der aktuellen PowerShell Instanz gültig. Wird diese beendet sind die erstellte Aliase nicht mehr verfügbar! Hierfür kann das [Profile](#Profile) Verwendet werrden um Aliase und andere Einstellungen/Cmdlets dauerhaft zu erstellen bzw. auszuführen.


Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 

Zeile 


## Profile

Profile...




## Aufgaben

### 1. Ermittle das Cmdlet vom Alias `gl` mittels dem Alias von `Get-Alias`

Selbst `Get-Alias` besitzt ein Alias, finde diesen heraus um damit zu ermitteln, welcher Cmdlet hinter `gl` steckt.

