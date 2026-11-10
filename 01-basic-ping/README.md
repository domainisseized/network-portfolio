# Lab 01: Basic Ping

**Objective:** Connect 2 PCs and verify connectivity using different cable types.

## Configuration
- PC1 (user1): 192.168.1.10 / 255.255.255.0
- PC2 (user 2): 192.168.1.11 / 255.255.255.0

## Test 1: Crossover cable (PC to PC)
Two like devices connected directly need a crossover cable. Both link lights are green.

![Crossover topology](Crossover%20Connection.png)

Ping from PC1 to PC2 succeeds with 0% loss.

![Crossover ping](Crossover%20Connection%20Ping.png)

## Test 2: Straight-through cable (PC to PC)
Ping fails. Like devices need a crossover cable, because a straight-through cable connects transmit to transmit.

## Test 3: Straight-through cables through a switch
PC1 and PC2 each connect to a 2960 switch with straight-through cables. All link lights are green.

![Switch topology](lab%201%20straight-through%20cable.png)

Ping from PC2 to PC1 succeeds. The first reply is slower because of the ARP lookup.

![Switch ping, first run](Screenshot%202026-11-10%20101731.png)

![Switch ping, second run](Screenshot%202026-11-10%20101844.png)

Switch port status, showing FastEthernet0/1 and 0/2 Up:

![Switch ports](Screenshot%202026-11-10%20102005.png)

## TL;DR:
Like devices need crossover cables; unlike devices need straight-through cables. The first ping through a switch is often slower while ARP resolves the MAC address.
