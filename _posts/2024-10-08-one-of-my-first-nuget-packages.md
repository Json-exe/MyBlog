---
layout: post
title:  "Eines meiner ersten NuGet Pakete"
date:   2024-10-08 13:00:00 +0200
categories: Programmierung
tags: Projekt
author: Luca
excerpt: In diesem Beitrag stelle ich mein NuGet-Paket "MudBlazor.SimpleIcon" vor, das es ermöglicht, alle Icons von SimpleIcons in MudBlazor-Projekten zu nutzen. Ich erkläre die Funktionsweise des Pakets, wie es erstellt wurde und wie es automatisiert veröffentlicht wird.
---

## Eines meiner ersten NuGet-Pakete!

Vor einiger Zeit, um genau zu sein am 8. Februar, habe ich das NuGet-Paket "MudBlazor.SimpleIcon" auf NuGet veröffentlicht.

Dieses Paket ist ein sehr simples Add-On für C#, Blazor und das Frontend-Framework [MudBlazor](https://mudblazor.com), mit dem ihr alle Icons von [SimpleIcons](https://simpleicons.org/) nutzen könnt. Dazu wird sogar die Standardfarbe als Kommentar über das jeweilige Icon geschrieben, sodass man einfach die Farbe implementieren kann. Ebenso steht die Lizenz des Icons in dem Kommentar.

Stand heute ist die aktuellste Version: 1.6.5.

## Funktionsweise

Ich habe ein kleines Skript mittels TypeScript geschrieben, das das npm-Paket von SimpleIcons nutzt und dann in eine C#-Datei alle wichtigen Informationen zu den Icons schreibt. Dabei wird auch sichergestellt, dass die Namen der Icons CamelCase sind.

Nachdem das Skript die C#-Datei erstellt hat, wird eine Solution, die diese Datei enthält, gebaut und dann als NuGet-Paket gepackt und hochgeladen.

Damit ich dies alles so einfach wie möglich automatisieren kann, habe ich eine Pipeline in Jenkins gebaut, der ich die Paketversion mitgeben kann, um dann eine neue Version des NuGet-Pakets zu erstellen.

Für alle weiteren Informationen, wie das Paket genutzt werden kann, wie der Code aussieht usw., schau doch in meinem GitHub-Repository vorbei oder klicke [hier](https://github.com/Json-exe/MudBlazor.SimpleIcons), um direkt dorthin zu kommen.

## Links

GitHub: [https://github.com/Json-exe/MudBlazor.SimpleIcons](https://github.com/Json-exe/MudBlazor.SimpleIcons)

Nuget: [https://www.nuget.org/packages/Json_exe.MudBlazor.SimpleIcons](https://www.nuget.org/packages/Json_exe.MudBlazor.SimpleIcons)