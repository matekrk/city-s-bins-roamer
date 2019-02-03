# city-s-bins-roamer
Best multiplayer with AI game ever!

City's bins Roamer : multiplayer game with AI for sustainable cities!

Goal: if you play as 'garbage' try to escape from Intelligent System of Bins!!If you play as 'bins' (audience) try to collect garbage!Idea: Player (garbage) can navigate around the city of Montreal (Microsoft Bing Maps). There is one place at the map that it is player's goal. They try to reach it before bins 'eat' you. But also, it has to avoid audience's goal!
Goal of audience is to prevent Player to reach player's goal. By placing bins they try to push player towards audience's goal.

Implementation: Because bins' signals are sometimes weak and noisy, we are using Martello's database which is useful in decision making (which provider should we trust more locally, and how much should we trust signal and how much our previous knowledge (somehow similar to AI concepts like particle filters etc.) This is how we analyse data provided by Martello in order to have knowledge about local signals in order to have better navigation throughout the city. 
By Rest API we could retrieve information about the city's map structure which is passed to pygame framework. All algorithms (navigation, AI's game style) are implemented from scratch. 

Therefore: Microsoft Bing Maps (+Rest API) + Python pygame + Flask + AI + Information Theory

For the future:
Combine everything:
- combine ability to make decision (about the signal) with navigation's algorithms.
- combine Bing Maps with pygame (style, retrieve data from map to have streets' layout etc.)
- combine by Flask data from Martello to Bing Maps so that they can contain information about signals' strentgh.
