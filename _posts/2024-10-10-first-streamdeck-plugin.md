---
layout: post
title:  "Mein erstes Stream Deck-Plugin!"
date:   2024-10-10 13:40:00 +0200
categories: Programmierung
tags: Projekt DevLog
author: Luca
excerpt: "In diesem Beitrag zeige ich, wie ich mein eigenes erstes Stream Deck-Plugin entwickelt habe, um Stream-Marker zu erstellen. Ich erkläre die Funktionsweise dahinter und warum ich zu dieser Idee kam. Am Ende teile ich das Ergebnis und den Code auf GitHub."
---

# Mein erstes Stream Deck-Plugin!

Gestern Abend habe ich mit einem Kollegen zusammen auf Twitch Raft gestreamt. Seit ein paar Tagen habe ich mit dem Streaming wieder angefangen und richte alles noch so ein wenig ein.

Ein Feature, das ich von Twitch ganz cool finde und unbedingt nutzen wollte, waren Stream-Marker. Also habe ich die Twitch-Erweiterung für mein Stream Deck heruntergeladen und wollte nun im Stream, Marker erstellen. Jedoch vergeblich.

Nach einer kurzen Recherche habe ich dann herausgefunden, dass man Marker nur erstellen kann, sofern man in den Twitch-Einstellungen aktiviert hat, dass Streams als VOD gespeichert und direkt veröffentlicht werden. Ersteres hatte ich bereits aktiviert, jedoch möchte ich nicht, dass meine VODs direkt veröffentlicht werden. Somit konnte ich die Marker von Twitch leider nicht verwenden.

## Problemlösung

Nach dem Stream habe ich dann ein wenig gegrübelt und mir gedacht: „Schreib doch einfach dein eigenes Stream Deck-Plugin, mit dem du Marker erstellen kannst!" Browser geöffnet und auf die offizielle Seite vom Stream Deck SDK navigiert. Dort habe ich mir dann erstmal angeschaut, wie man ein Plugin erstellt, welche Programmiersprache genutzt wird und welche Techniken.

Elgato nimmt hier TypeScript und Node.js für ihre Plugins. Also eben schnell ein Plugin-Projekt nach Dokumentation aufgesetzt und das Beispielprojekt ausgeführt. Et voilà, ich konnte auf meinem Stream Deck den Beispiel-Button hinzufügen.

Also habe ich mir den Code etwas genauer angesehen. Der Button und die Eigenschaften sind Standard-HTML gewesen. Die Funktionen des Buttons waren in einer separaten Datei. Stück für Stück habe ich mir dann Teile der Dokumentation und des Beispielcodes durchgelesen und angefangen, den Code so abzuändern, dass er meinen Bedürfnissen entspricht.

## Ergebnis und Funktion

Nach nicht mal allzu vielen Zeilen Code war mein Plugin bereits fertig. Insgesamt habe ich nicht mal eine Stunde gebraucht, um meine Funktion zu erreichen. Ich hatte nun einen Button, der die Zeit im folgenden Format anzeigte: `00:00:00`. Dazu gab es noch ein Datei-Feld, in dem man eine Textdatei auswählen konnte. Wenn man nun den Button einmal drückt, fängt dieser an hochzuzählen. Drückt man den Button erneut, setzt er sich wieder zurück. Hält man den Button länger gedrückt, wird der aktuelle Timestamp, der auf dem Button angezeigt wird, in die angegebene Datei geschrieben – mit einem Informationstext, den man optional noch festlegen kann.

Dieser Button liegt jetzt genau neben meinem „Stream starten"-Button, und ich muss ihn nur drücken, nachdem ich den Stream gestartet habe. Und schon kann ich mir Timestamps für meinen Stream erstellen, auch ohne meine VODs zu veröffentlichen. Natürlich ist der Button noch nicht perfekt, und ich werde ihn wahrscheinlich in Zukunft weiter optimieren. Ebenso kann es zu leichten Differenzen in den Timestamps von meinem Button und dem vom Stream kommen, aber dafür habe ich aktuell keine Lösung. Jedoch reicht mir das von den Features bereits.

Zum Ende hin noch eben ein GitHub-Repository erstellt und den Code dort hochgeladen.

Sowas erinnert mich immer wieder daran, dass Programmieren einfach verdammt cool ist.

## Informationen

GitHub: [https://github.com/Json-exe/StreamDeckPlugins](https://github.com/Json-exe/StreamDeckPlugins)

Vielen Dank fürs Lesen und noch einen schönen restlichen Tag! ^^