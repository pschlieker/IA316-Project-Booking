# Project of the IA316 Cours "AI &amp; E-Commerce"
Contextual Bandits for Booking.com optimizing the margin of booking.com

## Description
The general idea of the system is to recommend hotels for a given user. As on Booking.com the user will first enter its travel destination and the system will then present a featured hotel. As there's a lot of competition in the hotel booking industry, the goal is to have the user book the hotel right away. Hence we want to propose the perfect hotel.

## Feautures of Environment
* Limited room availability depending on hotel
* User preferences, which decide whether a user will book a hotel or not
* Partner Program which promotes certain hotels
* Different margins for different hotels

## Implemented Agents
* Random
* Adaptive Greedy
* Epsilon Greedy
* Thompson Sampling
* UCB
* Embedding Agent
  - Offline: Only trained once with historical data
  - Online / Offline: Trained with historical data and from time to time retrained with new data
  - Online: Switch between random exploration and exploitation with decreasing probability on exploration
* Hybrid Agent: Embeddings + Meta Information about user & hotels