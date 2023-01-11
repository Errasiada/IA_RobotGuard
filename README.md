# IA_RobotGuard
 
 Practice with behaviour trees. Modifying the NPC tree and adding two new behaviours:
 
 1.) The NPC will return to the last seen position of the player before Player fleed away.
 
 2.) NPC will only return to that position when HP is higher than 40%.
 
 First let's create a new tree inside _BotAI.BT_ called _tree "GoToLastPlayerPosition"_ and adding the new conditions requirements.
 
 ![image](https://user-images.githubusercontent.com/114673717/211861508-3dbaa41f-75c5-4a5b-8ad9-493e09f32005.png)
 
 The sequence of actions means that NPC will set its destination to the last position of the player while Health is not less than 40 and while not in Danger. Also, while the NPC is not _IsFleeingFromPlayer_, it will start attacking again.
 
 ![image](https://user-images.githubusercontent.com/114673717/211862308-d9eb0346-e0f4-45f3-933d-d60ead014fa8.png)

Sample of NPC fleeing after HP is 40 or less.

![flee](https://user-images.githubusercontent.com/114673717/211863404-ace91752-eef0-4d84-861c-c02d13faa1ec.gif)

Sample of NPC returning to last player's position after HP is greater than 40.

![flee2](https://user-images.githubusercontent.com/114673717/211863814-0f4c6833-519e-47b8-94dc-c16ae1e46d06.gif)
