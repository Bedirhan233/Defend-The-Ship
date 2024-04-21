# Defend-The-Ship

![GameSS](https://github.com/Bedirhan233/Defend-The-Ship/assets/114574131/37f0e564-c15f-4073-b065-5bea3f2cefcb)
### About the Game

Defend the Ship is a game where you must protect your ship from enemies attempting to destroy it. You command a robot that can repair the ship, gather metal to build a turret, or simply follow the player.

## Robot AI Command Logic

I used 'AI move to' for my logic. Based on player input on the robot it trigger the events that change the target variable, which sets the target for 'AI move to'. Basically, we choose what the robot should do.
![Capture](https://github.com/Bedirhan233/Defend-The-Ship/assets/114574131/d8f71cd0-dae2-400b-b119-e736cc51c4c0)
![Event](https://github.com/Bedirhan233/Defend-The-Ship/assets/114574131/ca7371f5-44d4-4934-a683-917d554a2718)




By doing that, the robot moves to those locations, gathers the necessary resources, and then returns to the station after a delay. For example, in the metal gathering system, I use a boolean to toggle the state. When it's false the robot moves to gather metal and the boolean is set to true. Then it returns to the station, adds the value to the system and the boolean changes to false after a delay.
![MetalHandlerEvent](https://github.com/Bedirhan233/Defend-The-Ship/assets/114574131/86ab75d8-c9d9-4a70-b9fd-493fe4e97842)
![FunctionForMetal](https://github.com/Bedirhan233/Defend-The-Ship/assets/114574131/a5142798-a2d7-4569-a8e5-2d16afc7fa05)



