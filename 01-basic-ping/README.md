# Lab 01: Basic Ping

**Objective:** Connect 2 PCs and verify connectivity.

## Configuration
- PC1: 192.168.1.10 / 255.255.255.0
- PC2: 192.168.1.11 / 255.255.255.0

## Tests
- **Test 1:** PC to PC with crossover cable. Ping succeeds.
- **Test 2:** PC to PC with straight-through cable. Ping fails (like devices need crossover).
- **Test 3:** PC to switch to PC with straight-through cables. Ping succeeds.

## Screenshots
**Crossover topology**

![Crossover topology](Crossover%20Connection.png)

**Crossover ping success**

![Crossover ping](Crossover%20Connection%20Ping.png)

**Straight-through (PC to PC) test**

![Straight-through test](lab%201%20straight-through%20cable.png)

## TL;DR
Like devices need crossover; unlike devices need straight-through type of cable.
