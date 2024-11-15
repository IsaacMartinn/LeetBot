<img width="638" alt="Screenshot 2024-11-04 at 9 35 32 AM" src="https://github.com/user-attachments/assets/af11bc1b-6bcd-41b9-a04f-f124265acf7e">

Inspiration
Solving Leetcode problems has been a key part of our journey in building coding skills and preparing for interviews. It’s given us exposure to a wide range of coding challenges and helped us sharpen our problem-solving abilities. However, doing it over and over can get a bit stagnant. After a while, the excitement fades, and it starts to feel like a chore. That’s where our idea comes in: a multiplayer game that integrates Leetcode challenges, turning problem-solving into something fun and competitive. Instead of just grinding through problems on your own, you can challenge friends, collaborate, and keep things interesting. This approach not only makes coding more enjoyable but also helps us stay motivated and continuously improve our skills in a more engaging way.

What it does
After entering a Leetcode username, players receive a custom robot character with a unique name generated using the Mistral AI API. The robot’s attribute scores—Punch, Kick, Blast, and Smash—are determined by the player's Leetcode performance. To boost these attributes, players can quickly solve Leetcode problems and earn bonus points. The game is a turn-based, two-player fighting match where opponents take turns attacking until one robot’s health is fully depleted.

How we built it
We started by defining the core features of what we wanted the project to look like: Robot characters with attributes such as Punch, Kick, Blast, and Smash abilities, and integrating these features with a Leetcode problem-solving environment to motivate users and reward them for their dedication and skill improvements.

The development of LeetBot combines several advanced technologies to create a dynamic and engaging multiplayer experience. The game's user interface is built using React, ensuring a responsive and interactive environment for players. Socket.IO is employed for real-time game interaction, enabling seamless communication and updates during gameplay. The CSS framework is utilized for styling, giving the game a polished and visually appealing look. To enhance the game's functionality, Mistral AI is integrated for generating LeetCode questions and usernames, while the LeetCode API is used to create and track player stats, such as progress, scores, and question completions based on difficulty levels. The backend of the game is powered by Flask, which supports the integration of WebSocket connections for real-time updates, ensuring that players' actions are reflected instantly within the game. This combination of frontend and backend technologies, including HTML, CSS, React.js, socket.io, Mistral AI, and the LeetCode API, allows Leetcode Robots to transform the traditional coding challenge experience into an engaging, competitive, and fun game.

Challenges we ran into
By using Mistral AI it takes longer to load, so when you call the API it takes longer for you to get your data back. We chose to research different models and find one that was more optimized for our needs. After users complete their Leetcode question it redirects you to another page, where it spits back the correct answer. This required creative thinking to maintain the same Socket.io connection throughout the process.

On the first night it took working for hours trying to get the multiplayer aspect of the game to work where we tried to get the calls back and forth between the players. At the start our process was trying to program it on our own which was a rigorous process and ultimately led us to a better way of going about the challenge. That's when we learned about the documentation called Socket.io which was used to enable real-time interactions between players. For example, when a player makes a move, that action is immediately sent to the server and then broadcasted to other players, ensuring that everyone sees the latest game state without delay. This was important for maintaining the flow and competitiveness of the multiplayer experience and making sure we created a successful working game. Another demanding aspect was ensuring the game functioned seamlessly on both screens and establishing a reliable connection between them.

Accomplishments that we're proud of
One of the most rewarding aspects of this hackathon was stepping out of our comfort zones and creating something new in such a short period. For many of us, it was our first time using this particular tech stack, and as newcomers to the hackathon scene, it was worthwhile to see our vision come to life. This experience was a great learning experience and was able to give us the confidence to tackle projects just like this!

More specifically, we started by looking at the documentation of socket.io which was completely new to us, since it was a new concept of trying to send the program information onto a different computer. Another achievement was when it came to working with React, it has an inheritance aspect similar to java but also had many differences, which we had to learn more about. When creating a session, it only works on a singular page and when on the website it can be seen that you are transferring from pages and there are all sorts of variables that are changing so keeping that session alive the entire time was something we were proud of being able to work through and understand.

What we learned
Throughout the development of the project, there were definitely some key takeaways and growth experiences we encountered as a team. Prior to this hackathon, we hadn't been exposed to many of the technologies used to create LeetBot. Given the 36-hour time constraint, we had to invest time to learn the fundamentals by watching tutorials and going over documentation to gain a solid understanding of the framework, enabling us to successfully create Leetbot.

One main principal we learned while participation in Ignition Hacks is appreciating the process and learning from our mistakes. For instance, by learning the harder principles and fundamentals of the code, and technicalities it allowed us to have smooth sailing when it came to working with the right technologies and tools.

What's next for LeetBot
Since there was a time constraint for this hack, if given the opportunity there are a variety of ways we would love to expand our game to the next level!

Here are some ideas we have for what's next!

Multiplayer enhancements: Add more multiplayer modes, such as team battles or tournaments to create a more collaborative and competitive environment.

AI integration: improve the AI opponents with more advanced algorithms that adapt to the player’s skill level, providing a more personalized and challenging experience.

