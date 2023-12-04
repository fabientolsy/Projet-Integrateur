# Projet-Integrateur

## Conception
- [ ] L'architecture doit respecter les concepts des réseaux commutés hiérarchiques (couches accès, distribution et coeur)
- [ ] Le réseau doit etre constitué de commutateurs, commutateurs multicouches et de routeurs
- [ ] Le réseau doit avoir des serveurs AAA et DHCP 

## Adressage
- [ ] Le réseau doit implenter la topologie double pile
- [ ] Tous les équipements doivent pouvoir gérer l'IPv4 et l'IPv6
- [ ] Créer un plan d'adressage (adresses des réseaux, plages d'adresses de ces réseaux, etc...)
- [ ] Fournir la topologie logique du réseau (il y faut les adresses réseaux, les indications pour les VLANs, etc)

## Redondance
- [ ] Implanter la redondance au niveau des équipements pour permettre une grande disponibilité du réseau
- [ ] Il doit y avoir une redondance au niveau des passerelles par défaut en utilisant le protocole HSRP

## Disponibilité
- [ ] Implanter Etherchannel entre certains commutateurs. Il faut determiner à auel endroit l'implanter et le justifier
- [ ] Implanter DHCP. Configurer des équipements (routeurs ou commutateur multicouche) et des serveurs pour offrir le service
- [ ] Seuls les serveurs et les équipements de réseau doivent avoir des adresses fixes
- [ ] Tous les PCs (en placer au moins un par VLAN) doivent obtenir leurs qdresses via DHCP

## Sécurité
- [ ] Implanter la sécurité des ports sur les commutateurs
- [ ] Le réseau doit contenir des Access-List autant en IPv4 qu'en IPv6
- [ ] L'authentification sur les équipements doit se faire en AAA à l'aide de serveurs
- [ ] Implanter soit un VPN IPsec ou un firewall ASA
- [ ] Implanter le DHCP snooping

## Routage
- [ ] Routage dynamique avec OSPF multizone
- [ ] Une zone par bulding + zone fédératrice
- [ ] Routage statique pour des routes récapitulatives
- [ ] Alléger le plus possible les tables de routages
- [ ] PPP entre les routeurs de la couche coeur avec CHAP
- [ ] Prévoir un lien par building vers un fournisseur d'accès et une route pour y diriger le trafic dédié à l'externe
