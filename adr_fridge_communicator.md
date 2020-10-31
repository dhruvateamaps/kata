# Title
Use of a separate component to communicate with smart fridge network

## Status
accepted

## Context
We need an ability to interface with the network of fridges  
This can be done by directly calling the individual fridge APIs from the calling component  
Another way of accomplishing communication with the fridges is through a separate dedicated component  

## Decision
We will use a separate dedicated component  

Hardcoding the API calls of a single type of smart fridge vendor creates vendor lock in at the technology layer   
Creation of a dedicated component enables handling any other vendor as well as interface with other devices  

## Consequences
This decision will require components to interface with the dedicated fridge component for fridge related information.  
