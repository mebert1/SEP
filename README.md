# Introduction

This project is a a server-based multiplayer game designed with and running on the Unity engine.

The game is a freely expandable learning platorm with the purpose of popularizing the advantages of gamification in education.



To run a first beta of the game, follow the steps below.



Language: **German**

Developers: 

- Lionel Damtew
- Marius Ebert
- Jens Niederreiter
- Elias Kupferschmitt

School: University of Applied Sciences Mittelhessen, Gießen, Germany (*Technische Hochschule Mittelhessen*)



Wiki: https://wiki.thm.de/SWT-P_SS_2018_Thunderstorm_Entertainment



_____




# Anleitung zum Starten des Spiels

## Auf lokalem Rechner:
1. In Unity unter Tools -> Setup -> Build All
2. Kommandozeile öffnen
3. `.\MasterAndSpawner.exe -batchmode -nographics -msfStartMaster -msfStartSpawner -msfMachineIp 127.0.0.1 -msfMasterIp 127.0.0.1 -msfExe ".\GameServer.exe"`\*

4. `.\Client.exe -msfMasterIp 127.0.0.1`

\*Hinweis:
Zum Beenden des lokalen Servers müssen die Unity-Instanzen manuell über den Task-Manager beendet werden.
## Auf Saturn:
1. In Unity unter Tools -> Setup -> Build Server for Linux
2. Dateien "GameServer.x86", "MasterAndSpawner.x86" und Ordner "GameServer_Data" und "MasterAndSpawner_Data" auf Server übertragen
3. .x86-Dateien ausführbar machen (chmod +x)
4. Server starten:
    1. Zwei Terminals öffnen
    2. `./MasterAndSpawner.x86 -msfStartMaster -logFile`
    2. `./MasterAndSpawner.x86 -msfStartSpawner -logFile`
5. Client starten:
    1. In Unity unter Tools -> Setup -> Build Client
    2. Client.exe starten

## Spielen:

1. "Play as Guest" oder Einloggen
2. "Start" klicken. Man tritt nun dem Lobby Raum bei
3. Auf das Spielen vorbereiten
    1. Eine Party erstellen und beliebig viele Spieler dieser Party beitreten lassen.
    2. In den Trigger gehen um mit seinen Mitspielern das Level zu betreten
4. Spielen :)
