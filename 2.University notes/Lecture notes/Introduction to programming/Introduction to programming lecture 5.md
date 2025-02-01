---
Date created: 2024-10-24 14:09
tags:
  - Type/Lecture_Note
  - Topic/Introduction_To_Programming
---

---

Een programma is correct indien het voldoet aan zijn specificatie.
- Pre-conditie (toestanden/voorwaarden waaronder je programma correct moet werken)
- Post-conditie (toestanden/voorwaarden waaraan he programma op het eind moet voldoen)

Specificatie = wat , niet hoe. Hoe= implementatie, na implementatie, verificatie.
- Voor alle toestanden die voldoen aan de preconditie, na het uitvoeren van de het programma, voldoen ook aan de post conditie.$$ \text{Pre}\implies \text{Post} $$
- We schrijven $$ \{ P \}\;p\;\{ Q \} $$
We focussen hier enkel op de corectheid van algoritmes van een bapaalde vorm, namelijk

*Initialisatie*
While *lus voorwaarde*
	*lus opdracht*
*opdrachten*

Axiomas:
1. Toekenningsaxioma:  Laat toe om correctheidsbewering af te leiden voor een toekennings odracht. Gegeven een toestandsbewering Q na een toekeningsopdracht. $$ X=E $$Vervang alle voorkomens van $X$ in $Q$ door $E$ , noteerd $Q[E\backslash X]$. Check de voorbeelden gwn

Regels:
1. Regels van het logisch gevolg: Obvious implicaties
2. Regel van het na elkaar uitvoeren: "Transitiviteit van correctheidsbewijzen"
3. Regel van voorwaardelijke opdrachten: "Breakdowns van voorwaardelijke opdrachten en bewijzen met regel 2"
4. Regel voor lussen: Bewijs in twee splitsen, eerst er vanuit gaan dat je lus eindigt, de andere is bewijzen dat de lus effectief eindigt.

