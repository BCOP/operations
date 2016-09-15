# Operations of Autonomous Systems on the Internet
A journeyman's guide to the formation and governance of the virtual sovereign.

```text
The Internet is not rocket science, it's more like running an old Russian nuclear reactor.
-- Erik L. Smit, Zylon Internet Services vof
```

## Introduction

There are many paths that can lead a person toward reading these words.

In the early days of the Internet, the formation of an Autonomous System (AS) was the domain of pioneers. An individual or an organization would venture bravely into the disconnected virtual wilderness, stake their claim to a unique AS number from a finite set of integers which would act as the virtual sovereign's name, procure a unique subnet of IP addresses from a well defined space that would act as its territory, and finally use these IP addresses to number its citizens, the hosts.

The virtual sovereign would then proceed to establish diplomatic relations with its neighbor ASes, known as peering relationships, or simply peering. These relationships would be typically governed by a peering agreement, formal or informal, that outlines the rights and obligations of each party.

Some peering agreements grant broad and equal rights to all parties, including reciprocal right of free passage for the citizen hosts of each party on the  other's territory (peering). Other relationships, primarily between a smaller and less established ASes and their larger neighbors could require the smaller party to compensate the larger one for the right of passage (paid peering).

Yet other virtual sovereigns specialized in forming a large number of peering relationships with ASes near and far, then selling the right of passage through  their own territory, as well as that of their network of peers (transit providers).

Today, the act of seeking Internet connectivity independence and establishing a new AS is primarily a revolutionary act. An individual or an organization might seek independence from existing ASes which accept (and often, at great effort, attract) host citizens, known as Internet service providers for a number of reasons.

The primary reason is often that of political independence. The modern service provider AS binds its host citizens to an elaborate code of conduct (the Acceptable Use Policy and Terms of Service), as well as to its own infrastructure choices and economic interests.

A secondary albeit related reason is that of economic advantage. Citizen hosts belonging to the same organization may often find themselves at a better negotiation position acting as an AS themselves rather than as citizens of a larger AS in which they may hold little influence.

Regardless of the reason, the decision to seek autonomy and independence carries with it both increased responsibilities and increased cost. The minimal commitment required to set up as an AS can be modest. It is possible to establish a minimal presence in the global default-free zone (DFZ) by simply subscribing for membership in a local Internet registry (LIR), requesting an AS number and an IP addresses subnet, then delegating all other tasks to an existing service provider AS.

This minimalistic approach, however, offers little or no advantage or independence. Each additional step toward independence carries increased cost and requires increased knowledge and experience - the procurement of DFZ-scale BGP routing equipment, lifecycle management of this equipment, negotiation of transit and peering relationships and their physical interconnection aspects, provisioning of services such as forward and reverse DNS, NTP and e-mail handling, proactive and reactive abuse handling, and many others.

This guide aims to structure and direct your journey through the formation and governance of the virtual sovereign. It lists resources, provides best practices, and discusses some common pitfalls.

## Governance

### Ministry of Interior

#### Business and Operations Support Systems

* [Issue Tracking Systems](Issue_Tracking_Systems.md)
* [Configuration Monitoring](Configuration_Monitoring.md)

### Ministry of Foreign Affairs

#### Peering Coordination

In the world of autonomous systems, peering coordination is the art of diplomacy. Being a broad topic covering the very essence of relationships between virtual sovereigns, fairly extensive research and resources are available on the subject. Few of them, however, are capable of replacing the intuition of a seasoned peering coordinator and capacity planner. As such, this art is still best learned through apprenticeship or ample practice.

* [DrPeering.net : Resources to make strategic peering decisions.](http://drpeering.net/index.php)
* [The Art of Peering: The Peering Playbook - Internet Society](http://www.internetsociety.org/sites/default/files/norton3_20100811.pdf)
