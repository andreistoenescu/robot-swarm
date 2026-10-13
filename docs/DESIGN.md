🇬🇧 **English** · [🇷🇴 Română](DESIGN.ro.md)

# 🤖 Robot Swarm – Design Document

> A distributed system of autonomous robots searching together for a common target.
>
> **Status:** draft · **Platform:** ESP32 + ESP-NOW · **Simulation:** Docker · **Language:** C++

---

## Contents

1. [Purpose and context](#1-purpose-and-context)
2. [Assumptions and limitations](#2-assumptions-and-limitations)
3. [Fault model](#3-fault-model)
4. [Architecture](#4-architecture)
5. [Robot behavior](#5-robot-behavior)
6. [Local state](#6-local-state)
7. [Messages](#7-messages)
8. [Decision rules](#8-decision-rules)
9. [Failure scenarios](#9-failure-scenarios)
10. [Configurable parameters](#10-configurable-parameters)
11. [Open questions](#11-open-questions)

---

## 1. Purpose and context

The project implements a **distributed system of autonomous robots** that
search together, as fast as possible, for a target located in a room. The
target is a **static** source of a weak signal, and the search space is a room
of at most **10 × 10 m**.

The system is **fully decentralized**: there is no leader or central
coordinator. Each robot chooses its next action on its own, based on the
information exchanged with the others. To coordinate the search, the robots
jointly build a **shared map of the signal intensity** across the room.

| | |
|--|--|
| 🎯 **Target** | weak signal source, static |
| 📐 **Space** | room of at most 10 × 10 m |
| 🕸️ **Architecture** | fully decentralized, no coordinator |
| 🗺️ **Coordination** | shared map, synchronized between robots |

---

## 2. Assumptions and limitations

_To be written._

## 3. Fault model

_To be written._

## 4. Architecture

_To be written._

## 5. Robot behavior

_To be written._

### 5.1 Startup and discovery
### 5.2 Exploring the own zone
### 5.3 Signal-guided assistance
### 5.4 Target verification
### 5.5 Stopping

## 6. Local state

_To be written._

## 7. Messages

_To be written._

## 8. Decision rules

_To be written._

## 9. Failure scenarios

_To be written._

## 10. Configurable parameters

_To be written._

## 11. Open questions

_To be written._
