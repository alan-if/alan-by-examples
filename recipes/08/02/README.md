# 8.2. Ships, Trains and Elevators

Inspired by same-named section of _[The Inform Recipe Book]_.


-----

**Table of Contents**


<!-- MarkdownTOC autolink="true" bracket="round" autoanchor="false" lowercase="only_ascii" uri_encoding="true" levels="1,2,3,4" -->

- [Introduction](#introduction)
- [Implementation Overview](#implementation-overview)
    - [Common Elements](#common-elements)
    - [Variable Features](#variable-features)

<!-- /MarkdownTOC -->

-----


# Introduction

This section deals with transportation vehicles which can be entered by the hero (and other actors) and are big enough to be self-contained locations (not nested) — unlike a car, a horse or a bicycle, which are usually visible in a location.

The main difference is that when an actor enters a ship, a train or an elevator, it's as if it entered another room altogether — although you can see the train from the station platform, you don't expect the train passengers to be in scope from the platform (i.e. visible and possible to interact with); whereas if an NPC mounts a horse you'd expect that actor and the horse to be viewable and in the scope when the player is at the location.

Ships, trains and elevators should have enough dissimilar elements to constitute a base example for any other vehicles belonging to this category.

# Implementation Overview

We'll refer to the act of entering such vehicles as _boarding_ them, and employ _disembarking_ to indicate the act of leaving them, and _travelling_ to indicate the transportation journey inside them.

## Common Elements

Because of the above features, this type of vehicles will be implemented as independent `location` instances (i.e. not nested in an outer location populated by actors) with exits that vary — i.e. after the vehicle has travelled, traversing backward the exit used to board the vehicle will lead to a different location than the original boarding location.

Furthermore, once the vehicle has started travelling, it should no longer be available for boarding at the initial location, but might become available for boarding at other locations — the final destination and any intermediate stops, if the vehicle journey admits them.
Therefore, any location at which the vehicle might be boarded and/or disembarked should also allow conditional `Exit` statements, depending on whether the vehicle is currently available.

## Variable Features

Depending on the nature and function of the vehicle being implemented, and the type of journey it offers, we might have a vehicle that travels for many turns, without being possible to embark or disembark it until the next stop (e.g. a boat cruise, a train), or we might have a vehicle offering a different stop at each turn (e.g. a train, a bus or an elevator).

Whether we wish the journey to be immediate, or to offer intervals between the various stops depend on what we want to achieve — in a long cruise, the boat might become a main setting of the adventure, lasting many turns, whereas an elevator is most likely going to merely connect different floors. A train might be just a gimmick to quickly move around a map that involves different cities, and we don't expect anything meaningful to happen on the train; but just like a boat, it could become a place of action, if we wish so.

While an elevator is always going to be a single location, a train might consist of multiple locations chained together, and a ship could either be just a small boat or a huge transatlantic like the Titanic, offering a fully fledged adventure set, with hundreds of suites and cabins, various restaurants, shops, and all sorts of comforts.

We also need to know/decide who controls the journey and how:

- Is there a driver, a captain, or is the journey controlled by the player?
- How do you control the vehicle? by speaking to its driver? by taking control of it by some steering device? by pressing buttons? or is the vehicle journey predetermined by some computerized program (e.g. a subway train)?
- Is the vehicle free to move around as it wishes (e.g. a boat, a bus)? or is it's journey constrained by physical constraints (like rails for a train, or the shaft for an elevator)?


<!-----------------------------------------------------------------------------
                               REFERENCE LINKS
------------------------------------------------------------------------------>

[The Inform Recipe Book]: http://inform7.com/book/RB_8_2.html "View section '8.2. Ships, Trains and Elevators' of 'The Inform Recipe Book' online"


<!-- EOF -->