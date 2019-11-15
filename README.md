#### Ερώτημα 2
---
Ζητείται να επαληθεύσουε τα βασικά χαρακτηριστικά του 1ου ερωτήματος εξετάζοντας τα αρχεία **_config.ini_** και **_confing.json_**.

* Για το σύστημα :

```
i.[system.clk_domain]
clock=1000 

```
Από το _clock_ το οποίο είναι 1000 picoseconds προκύπτει πως η συχνότητα του επεξεργαστή είναι **_1GHz_**

```
ii.[system.voltage_domain]
voltage=3.3 V
```
* Για τον επεξεργαστή :

```
i.[system.cpu_cluster.clk_domain]
clock=250

```

Από το _clock_ το οποίο είναι 250 picoseconds προκύπτει πως η συχνότητα του επεξεργαστή είναι **_4GHz_**
```
ii.[system.cpu_cluster.cpus]
type=MinorCPU
```

```
iii.[system.cpu_cluster.cpus]
numThreads=1
``` 
Συμβολίζει τον αριθμό των πυρήνων ,  που στην περίπτωσή μας είναι 1.

```
iv.[system]
mem_mode=timing
```
```
v.[system.cpu_cluster.voltage_domain]
voltage=1.2 V
```
* Για την **_DRAM_** :

```
i.[system]
mem_ranges=0:2147483647
```
Διαιρώντας την τιμή **2147483647** με το (1024)^3 προκύπτει το μέγεθος της **_DRAM_** : **_2GB_** .

```
ii.Ο τύπος δεν αναγράφεται στο αρχείο.
```
```
iii.


