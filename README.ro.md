[🇬🇧 English](README.md) · 🇷🇴 **Română**

# 🤖 Robot Swarm

**Un roi descentralizat de roboți ESP32 care caută împreună o țintă, fără coordonator central.**

Proiect de licență axat pe **sisteme distribuite**: fiecare robot decide singur, folosind doar
ce aude de la ceilalți pe un canal radio care pierde mesaje.

> 🚧 **Stare:** faza de proiectare. Încă nu există cod: întâi se specifică comportamentul,
> apoi structura fișierelor, apoi implementarea.

## ✨ Idei principale

- 🕸️ **Fără lider.** Fiecare robot aplică aceleași reguli pe aceleași date și ajunge la aceleași decizii.
- 🗺️ **Hartă comună a semnalului**, replicată pe fiecare robot și combinată cu `max` (un CRDT), deci
  mesajele pierdute, dublate sau reordonate nu strică nimic.
- 💓 **Heartbeat-uri** pentru membership și detecția defectelor; roboții pot muri sau reporni oricând.
- 🧩 **Împărțirea muncii după rang:** camera e împărțită în zone, reîmpărțite când apar sau cad roboți.
- ✅ **Terminare sigură:** ținta e declarată găsită doar după ce un al doilea robot o confirmă,
  iar vestea se răspândește prin gossip.

## 🛠️ Platformă

| | |
|--|--|
| **Hardware** | ESP32 |
| **Radio** | ESP-NOW (broadcast, fără confirmări) |
| **Simulare** | mai mulți roboți virtuali în Docker, același cod de logică |
| **Limbaj** | C++ |

## 📚 Documentație

- [Document de proiectare](docs/DESIGN.ro.md) ([English](docs/DESIGN.md))
