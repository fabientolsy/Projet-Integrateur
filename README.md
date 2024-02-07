# Projet integrateur

## Le projet
Le but du projet est de créer un réseau pour une entreprise fictive qui possède deux batiments. Ces batiments sont comportés de 3 étages et 2 sous-réseaux par étage chacun. Le principe étant de rendre le tout fonctionnel et sécurisé, même si un ou des équipement(s) tombe(nt) en panne. J'ai réalisé cela en respectant 6 aspects de la réseautique:
- Conception
- Adressage
- Redondance
- Disponibilité
- Sécurité
- Routage
  
## Conception
- [x] L'architecture du réseau respecte les concepts des réseaux commutés hiérarchiques (couches accès, distribution et coeur).
- [x] Le réseau est constitué de commutateurs, commutateurs multicouches et de routeurs.
- [x] Le réseau possède des serveurs DHCP.

## Adressage
- [x] Le réseau implente la topologie double pile.
- [x] Tous les équipements peuvent gérer l'IPv4 (IPv6 en cours).
- [x] Un plan d'adressage (adresses des réseaux, plages d'adresses de ces réseaux, etc...) et une topologie logique du réseau (il y faut les adresses réseaux, les indications pour les VLANs, etc) sont disponibles dans la documentation.

## Redondance
- [x] La redondance est implementer au niveau des équipements pour permettre une grande disponibilité du réseau.

## Disponibilité
- [x] Le DHCP est implementer dans les deux batiments. Un serveur possède les ègles et les commutateurs multicouche précisent le sous-réseau des postes pour que les serveurs donnent une adresse IP adéquate.
- [x] Seuls les serveurs et les équipements de réseau ont des adresses fixes.
- [x] Tous les PCs (en placer au moins un par VLAN) obtiennent leurs adresses via DHCP.

## Sécurité
- [x] Le réseau contenir des Access-List en IPv4 (IPv6 en cours).

## Routage
- [x] Routage dynamique avec OSPF multizone
- [x] Une zone par bulding + zone fédératrice
- [x] Routage statique pour des routes récapitulatives
- [x] Alléger le plus possible les tables de routages
- [x] PPP entre les routeurs de la couche coeur avec CHAP
