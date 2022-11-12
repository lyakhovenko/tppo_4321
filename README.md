# tppo_4321
**smart_lamp** is the software designed to control the brightness and color of the lamp. It is developed based on Python. This app has 2 sides: server and client.

---

## Table of contents

1.  [ Overview ](#overview)
2.  [ Dependencies ](#dependencies)
3.  [ Installation ](#installation)
4.  [ Run ](#run)
5.  [ Support ](#support)


---

<a name="overview"></a>
## 1. Overview

This app has 2 sides: server and client. 
A service that monitors changes in the state of a smart lamp, simulated by a local file, and receives / transmits requests and responses via a network control protocol.
A client program for managing the device through the service (and checking the operation of the service).

---

<a name="dependencies"></a>
## 2. Dependencies

Basic:<br>
- [Python (>=3.8)](https://www.python.org/)
- datetime
- os
- sys
- re

Third-party:<br>

- socket
- json

---

<a name="installation"></a>
## 3. Installation

Steps:

1. git clone https://github.com/lyakhovenko/tppo_4321.git or download ZIP
2. cd tppo_4321

---

<a name="run"></a>
## 4. Run
1. Make the files executable
```
chmod +x tppo_client_4321.py
chmod +x tppo_server_4321.py
```
2. Start the service
```
./tppo_server_4321.py
```
3. Start the client file with the right keys:

    3.1. ```-i``` is a key for getting information about lamp state.
    
    3.2. ```-b```, ```-c``` is keys for setting the brightness and color of the lamp. 
      
      Brightness - glow intensity (0 .. 10 conditional units). 
      
      Color - glow color in RGB format (three octets separated by commas)

For example:
```
./tppo_client_4321.py -b 0 -c 0,0,0
./tppo_client_4321.py -i
```
---

<a name="support"></a>
## 9. Support

Reach out to me at one of the following places!


---

