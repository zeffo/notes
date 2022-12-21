
# Buses

> Buses are wires which help transfer data across the CPU and memory.


## Parallel vs Serial

| **Serial**                          | **Parallel**          |
| ---------------------------------- | ----------------- |
| Slow                               | Fast              |
| More Distance = More Cost          | Cheaper           |
| More Frequency = More Interference | Less Interference |


## Conventional Buses

1) Local / System: CPU <--> Main Memory
2) Frontside: CPU <--> Chipset (eg NorthBridge)
3) Backside: CPU <--> L2 Cache
4) Memory: Chipset <--> Main Memory
5) AGP[^1] (Accelerated Graphics Port): Chipset <--> GPU

[^1]: AGP has been mostly phased out in favor of *PCI Express* since 2004.

## Measurements

> **WIDTH**: Total number of wires in a bus.

> **BANDWIDTH**: Maximum amount of data that can be transferred per unit time.

## Typical Buses

| **Name**     | **Bits** | **Speed** (Mbit/s) |
| ------------ | -------- | ------------------ |
| 16x ISA      | 16       | 15.9               |
| EISA         | 32       | 31.8               |
| VLB          | 32       | 127.2              |
| PCI          | 32       | 127.2              |
| 64x PCI 2.1  | 64       | 508.6              |
| AGB 8x       | 32       | 2133               |
| USB 2        | 1        | 1.5 / 12 / 480     |
| Firewire 400 | 1        | 400                |
| PCI-E 16x v2 | 16       | 8000               | 

