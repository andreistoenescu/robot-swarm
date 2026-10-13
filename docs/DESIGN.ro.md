[🇬🇧 English](DESIGN.md) · 🇷🇴 **Română**

# 🤖 Robot Swarm – Document de proiectare

> Sistem distribuit de roboți autonomi care caută împreună o țintă comună.
>
> **Stare:** în redactare · **Platformă:** ESP32 + ESP-NOW · **Simulare:** Docker · **Limbaj:** C++

---

## Cuprins

1. [Scop și context](#1-scop-și-context)
2. [Presupuneri și limitări](#2-presupuneri-și-limitări)
3. [Modelul de defecte](#3-modelul-de-defecte)
4. [Arhitectura](#4-arhitectura)
5. [Comportamentul unui robot](#5-comportamentul-unui-robot)
6. [Starea locală](#6-starea-locală)
7. [Mesaje](#7-mesaje)
8. [Reguli de decizie](#8-reguli-de-decizie)
9. [Scenarii de defect](#9-scenarii-de-defect)
10. [Parametri configurabili](#10-parametri-configurabili)
11. [Probleme deschise](#11-probleme-deschise)

---

## 1. Scop și context

Proiectul implementează un **sistem distribuit de roboți autonomi** care caută
împreună, cât mai rapid, o țintă aflată într-o încăpere. Ținta este o sursă
**statică** de semnal slab, iar spațiul de căutare este o cameră de cel mult
**10 × 10 m**.

Sistemul este **complet descentralizat**: nu există un lider sau un coordonator
central. Fiecare robot își alege singur următoarea acțiune, pe baza
informațiilor schimbate cu ceilalți. Pentru a coordona căutarea, roboții
construiesc împreună o **hartă comună a intensității semnalului** în cameră.

| | |
|--|--|
| 🎯 **Țintă** | sursă de semnal slab, statică |
| 📐 **Spațiu** | cameră de cel mult 10 × 10 m |
| 🕸️ **Arhitectură** | complet descentralizată, fără coordonator |
| 🗺️ **Coordonare** | hartă comună, sincronizată între roboți |

<!-- TODO (student): paragraful despre accentul pe sisteme distribuite, problemele și platforma -->

---

## 2. Presupuneri și limitări

_De scris._

## 3. Modelul de defecte

_De scris._

## 4. Arhitectura

_De scris._

## 5. Comportamentul unui robot

_De scris._

### 5.1 Pornire și descoperire
### 5.2 Explorarea zonei proprii
### 5.3 Ajutor ghidat de semnal
### 5.4 Verificarea țintei
### 5.5 Oprire

## 6. Starea locală

_De scris._

## 7. Mesaje

_De scris._

## 8. Reguli de decizie

_De scris._

## 9. Scenarii de defect

_De scris._

## 10. Parametri configurabili

_De scris._

## 11. Probleme deschise

_De scris._
