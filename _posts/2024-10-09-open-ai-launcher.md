---
layout: post
title:  "OpenAI-Launcher"
date:   2024-10-09 10:00:00 +0200
categories: Programmierung
tags: Projekt
author: Luca
excerpt: In diesem Beitrag wird der OpenAI-Launcher vorgestellt, ein Projekt, das die Nutzung von OpenAI-APIs wie GPT, DALL-E und Whisper demonstriert. Ich beschreibe die Motivation hinter dem Projekt, die implementierten Features und die verwendeten Technologien. Zudem werden Screenshots der Anwendung und ein Link zum GitHub-Repository bereitgestellt.
file-slug: "openailauncher"
---

## Der OpenAI-Launcher!

Der OpenAI Launcher war eines meiner ersten Projekte. An diesem Projekt habe ich mich mit OpenAI und deren API befasst. Auslöser hierfür war, dass ich Gratis-Guthaben hatte und mir einmal anschauen wollte, wie APIs funktionieren und wie einfach es ist, Künstliche Intelligenz selbst in ein Projekt einzubauen. Dabei habe ich die größten KI-Schnittstellen von OpenAI genutzt: GPT und DALL-E.

## Features

Die Features sind für dieses Tool sehr simpel gewesen:

1. Chat: Ein Chat-ähnliches Interface wie bei ChatGPT. Man konnte unterschiedliche Chats erstellen und dort über verschiedenste Themen mit dem in den Einstellungen ausgewählten Modell chatten.
2. DALL-E 2: Hier konnte man ein Prompt eingeben, eine Bildgröße und die Anzahl an Bildern auswählen, die generiert werden sollten. Diese wurden dann darunter direkt als Vorschau angezeigt und man konnte diese speichern.
3. Whisper: OpenAIs Speech-to-Text-KI hat auch eine Integration bekommen. Hier konnte man auswählen, ob man eine Transkription oder Übersetzung wollte. Dann hat man nur noch die Audio-Datei hochgeladen und optional noch die Quellsprache ausgewählt. Nach kurzer Ladezeit hat man dann die Ausgabe in einem Textfeld angezeigt bekommen.

All dies funktionierte natürlich mit dem eigenen API-Token, den man in den Einstellungen festlegen konnte.

Es gibt sogar die Möglichkeit, die Token-Anzahl für die Chats einzustellen, um das Limit des gewählten Modells nicht zu überschreiten.

## Technologien

Gebaut habe ich diese App mit der Programmiersprache C# und dem .NET-Framework. Für die UI kam WPF zur Hilfe mit einem Frontend-Framework namens Material-Design-In-XAML-Toolkit, um auch ein schönes Material Design zu gewährleisten.

## Showcase

Hier ein paar Bilder, wie das Projekt aussieht:

![Chat Fenster]({{ site.image_assets_path | append: page.file-slug | append: '/OpenAI-API-Wrapper_ntw4apyBBp.png' | relative_url }})

![Whisper Fenster]({{ site.image_assets_path | append: page.file-slug | append: '/OpenAI-API-Wrapper_Q6tY3Sr2c4.png' | relative_url }})

![Dall-E Fenster]({{ site.image_assets_path | append: page.file-slug | append: '/OpenAI-API-Wrapper_4FG6sqbFOG.png' | relative_url }})

## Weitere Informationen

| GitHub Repository: [https://github.com/Json-exe/OpenAI-Launcher](https://github.com/Json-exe/OpenAI-Launcher)
| Erster Commit: 13. März 2023
| Letzter Commit: 31. März 2023