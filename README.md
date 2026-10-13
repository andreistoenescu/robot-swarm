🇬🇧 **English** · [🇷🇴 Română](README.ro.md)

# 🤖 Robot Swarm

**A decentralized swarm of ESP32 robots that search together for a target, with no central coordinator.**

Bachelor's thesis project focused on **distributed systems**: each robot decides on its own,
using only what it hears from the others over a lossy radio channel.

> 🚧 **Status:** design phase. No code yet: the behavior is specified first, then the file
> structure, then the implementation.

## ✨ Key ideas

- 🕸️ **No leader.** Every robot runs the same rules on the same data and reaches the same decisions.
- 🗺️ **Shared signal map**, replicated on every robot and merged with `max` (a CRDT), so lost,
  duplicated or reordered messages do no harm.
- 💓 **Heartbeats** for membership and failure detection; robots may die or reboot at any time.
- 🧩 **Work split by rank:** the room is divided into zones and re-divided when robots join or fail.
- ✅ **Safe termination:** a target is declared found only after a second robot confirms it,
  and the news spreads by gossip.

## 🛠️ Platform

| | |
|--|--|
| **Hardware** | ESP32 |
| **Radio** | ESP-NOW (broadcast, no acknowledgements) |
| **Simulation** | multiple virtual robots in Docker, same logic code |
| **Language** | C++ |

## 📚 Documentation

- [Design document](docs/DESIGN.md) ([Română](docs/DESIGN.ro.md))
