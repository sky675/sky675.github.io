---
title: "OASIS 2 Changelog (1db8accffffcab4efec1224c0465de80903d2fa9)"
toc: true
toc_label: Changelog
full-width-toc: true
noindex: true
nopage: true
---

## Balancing
- reduce base stealth threshold for basic daemon [1db8acc]

## Bugfixes
- combat floor would keep getting its difficulty-buffed hp reset [51e7884]
- item for shield program was pointing towards the speed program (rabbit) [4459438]
- when daemon is set to null, call layer's disable func for it so it doesnt persist if it was active when the scene was left [0d64309]
