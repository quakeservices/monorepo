# Overview

This project as an attempt to replicate the idSoftware master server for Quake 2 (satan.idsoftware.com) in Python 3.

Core goals:
-  Respond to queries from clients such as qstat
-  Respond to queries and updates from Quake 2 servers
-  Support for protocol 35, 36, and 37
-  Be extensible enough to support other idTech engines/games
-  REST powered Web UI
-  Completely automated deployments

Stretch goals:
-  Support all common Quake, Quake 2, and Quake 3 derived servers and clients
-  Aggregation of existing master server lists
-  Multiregion support
-  GraphQL endpoint 
-  Support IPv6

# Requirements

Minimum requirements:
- Python 3.6+
- Docker
- DynamodDB

# Deployment

Deploying to ECR is done manually at this point.

All additional resources are handled by the [deployment repo](https://github.com/quakeservices/master_deploy)

# Contributing

Pull requests welcome!

Please raise issues via the GitHub issue tracker

This license for this project is GNU General Public License v3.0

Tab = 4 spaces

# Documentation

A lot of this was made considerably easier by the folks before me who documentation and researched the aspects of the Quake 2 networking stack. Below is a list of URLs I found useful while undertaking this project:

- [Quake 2 source code](https://github.com/id-Software/Quake-2)
- [Quake 2 source code review](http://fabiensanglard.net/quake2/index.php)
- [Quake Stat](https://github.com/multiplay/qstat)
- [Q2Pro source (protocol 36)](https://github.com/AndreyNazarov/q2pro)
- [R1Q2 (protocol 37) documentation](https://r-1.ch/r1q2-protocol.txt)
- [R1Q2 source (protocol 37)](https://github.com/tastyspleen/r1q2-archive)
