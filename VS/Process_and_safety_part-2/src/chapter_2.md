# Sequence diagram

Deze sequence diagram is een combinatie van twee, hier word namelijk weergegeven hoe de functie samen met de twee processen werkt.

```plantuml

@startuml
Gebruiker -> Proces_1 :Power on



Proces_1 -> Proces_2 : water opwarmen


Proces_1 -> Functie : Spoelen machine

Functie --> Proces_1  : machine gespoeld

Proces_2 --> Proces_1 : water opgewarmd

Proces_1 -> Proces_1 : Bonen aanwezig en melk aanwezig en voldoende water

Proces_1 -> Proces_1 : beker aanwezig

Gebruiker ->Proces_1 : start

Proces_1 -> Proces_1 : Melk word verwarmd en bonen gemalen

Proces_1 -> Proces_1 : Melk word verwarmd en gepompt

Proces_1 -> Proces_1 : water word door bonen gepompt

Proces_1 -> Proces_1 : kop koffie kan gepakt worden


@enduml