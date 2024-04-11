<h1 aligh="left">Welcome! ☕ </h1>
<H6>This is a mini Knowledge Graph of the characters in *Game of Thrones*, based on the storyline of Season 1 (Spoiler Alert ⚠️). </H6>
<p>Programmed with *Protégé 5.6.3*</p></br>
![Animation](C:\Users\yixin\Desktop\Workspace\Personal GitHub Repos\mini-GOT-ontology\Images\ned_stark.jpg")


# ⚔Classes⚔
###### Three main Classes are defined:
- House
- Person
  - Bastards
  - Rightful_heir
  - Claimed_rightful_heir
  - Crown_members
	- Concil
    - King
    - Kings_guard
    - Queen
  - Lord
- Town

# ⚔Instances⚔
Name of houses, persons and towns in the series
All characters in the Knowledge Graph are assumed *alive*.

# ⚔Relations⚔
Aligned with the storyline of Season 1, some of the notable relations are:
**Explicit:** 

- Assignment: 
    1.	Every person belongs to a House (Even Bastards!) - they might not be a direct member of that house family, but they might still live on their land under their regime!
    2.	Every House has a capital city, namely Main Town
- Disjointness: Some characters claimed their rights of inheritance of Iron Throne but do not have the rights based on the Law of Westeros. Therefore, *rightful_heir* and *claimed_rightful_heir* are disjoint with each other. 
Similarly, Some person might be married with another person but NOT necessarily in love with each other, and vice versa (So sad, huh?). Therefore, *marriedWith* is disjoint with *inLoveWith*

**Implicit**:
-   Equivalence: Every person is a rightful heir if raised by a King
-	King’s Guard: A person is a King’s Guard if a person is a crown member AND serves a king. When this relation is given to a person, the person will be assigned to Kings_guard by the Reasoner
-	Marriage: If A married with B, then B is of course married with A!

# ⚔Future work⚔
- *Is my favorite person died?* Implement a mini Ontology of other seasons, expanding from the version of *Season 1* by introducing a *live status* relation for each character. Allow query 
of the aliveness of a person at a given season!
- *Who killed my favorite guy?* Introduce a relation of who killed who
- *Which battles I have been to?* Introduce notable battles and those who fought in the battle! 
- *Magic creatures?* There exists magic creatures in the story, some owns and loves them, some battles against them! - Introduce them in the Ontology


