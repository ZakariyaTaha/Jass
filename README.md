The goal of this year's project, named Javass, is to write a program to play a variation of the famous Jass game. 
Jass is a very popular card game in Switzerland — where it is often referred to as a national sport — and in other neighboring countries, and is close to belote and other similar games.<br>

<br>
To run the game you need to determine how you want to play, and write in the "Arguments" tab in "Run Configurations":
<li>The first 4 arguments are the players, h corresponds to human, s to simulated player, and r to remote player. <br>
You can give a combination of 4 players written this way : h:<name>, s:<name>:<Algorithm number of iterations>, r:<name>:<IP>, where what's between <> is optional.</li>
<li>The 5th argument is optional and gives a seed to the program.</li>

<br>
Thus, the program can be launched in many way, some of which:
<li>Play locally against 3 simulated players : Run configurations -> in arguments put "h s s s"</li>
<li>Play locally 2 players against 2 simulated players : Run configurations -> in arguments put "h s r s"</li>
<li>Play locally 1 player against 2 simulated players and a remote player (better be in a private network or can fail): Run configurations -> in arguments put "h s r::IP s" with IP being the remote player IP, and in the LocalMain class change hostname to the remote IP</li>
<br>
