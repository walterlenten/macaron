# macaron
A "Phone Link" type app for Linux.

# Macaron

**Macaron** is an early-stage, experimental Linux application aiming to replicate Phone Link–style integration with iPhones over Bluetooth. The goal is to provide notifications, SMS, and phone call functionality on Linux desktops—starting with Fedora and GNOME.

---

## About This Project

This is a very beta, proof-of-concept project and a new personal venture for me (Asher). Apple’s Bluetooth protocols for SMS and calls are proprietary and heavily restricted, so this app is a first step toward bridging that gap on Linux.

Expect rough edges, limited features, and frequent changes as I explore how best to implement these capabilities.

---

## Current Features (and Limitations)

- Receives iPhone notifications using Apple Notification Center Service (ANCS) over BLE
- Basic Bluetooth pairing management
- Prototype support for SMS and phone call protocols (MAP and HFP) is experimental and incomplete
- GTK 4 frontend using PyGObject for a native GNOME experience

---

## Why Macaron?

Apple tightly controls iPhone Bluetooth interactions, leaving Linux users without easy access to SMS and call integration. Microsoft’s Phone Link on Windows works through a private partnership with Apple.

Macaron is an open-source attempt to create similar functionality on Linux, starting small and growing with community input.

---

## Installation

*(Installation steps coming soon as the project matures.)*

---

## Development

Contributions and feedback are welcome but please keep in mind this is early-stage and experimental.

### Requirements

- Fedora (preferred)
- Python 3.10+
- BlueZ Bluetooth stack
- PyGObject (GTK 4 Python bindings)
- dbus-python

### Running in development

```bash
pip install -r requirements.txt
python -m macaron.main
