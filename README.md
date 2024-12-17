# ChatGPT-Think-Alouds: Prompts and Knowledge Files

This repository aims to provide supplementary materials for the research paper titled 'GPT-Think-Alouds: Analyzing Player Emotion in VR Platformer Games via LLMs'.

We utilize LLMs to aid in the process of game testing. In our experiments, players play three VR games while thinking aloud. Their gameplay footage and audio are reviewed by our ChatGPT powered bot for emotion analysis. Our bot creates estimations on six emotions and perceived difficulty.

We utilize prompt engineering techniques to task our bot to conduct emotion analysis on players playing a VR game via the media provided. Each game had a similar prompt, as all detailed similar output expectations, with minor modifications per-game. The prompts outline important information such as what to expect (VR game), literature to take as reference for emotion analysis, creativity (prefer consistency), and output format.

### Prompts
- **InstructionsG1.txt**: Instructions for game 1 - 'Why did the chicken cross the road'.
- **InstructionsG2.txt**: Instructions for game 2 - 'Test your reflexes'.
- **InstructionsG3.txt**: Instructions for game 3 - 'Test the heights'.


Knowledge files are separately fed into the bot depending on which game is being analyzed. These files aid the bot in advancing its contextual understanding of the game scene and events. These files are crucial as they help reduce inccorect judgements and/or hallucinations.

### Knowledge Files
- **Game Description G1.txt**: Description of game 1 outlines the goal and important gameplay events such as crossing the street, oncoming car traffic, getting hit by car. It is important that the bot is able to visually distinguish game events as it can make the mistake of misinterpreting movement and events. For example, if the bot does not know that all cars are moving, it may presume cars are still in each frame. Additionally, game-specific animations such as the player floating up when they get hit is an important peice of information to help decipher key events. Specific for game 1, previous knowledge on difficulty metrics were also fed. Although the bot was not informed on which level it is watching, the description file outlined the differences in each level and how players on average perceived difficulty using data from a previous study.
- **Game Description G2.txt**: Description of game 2 outlines the various game objects and what they mean to the player. It also outlines negatives of objects such as obstacles to create an understanding that hitting these objects will slow the player down. It also describes the ways in which players try to win (collecting coins) and how they can do this with their body and hands, to make assessment of performance clearer. It also describes the potential levels briefly.
- **Game Description G3.txt**: Description of game 3 outlines the goal and level differences. It describes different difficulty inducing game events. It also describes visual queues to know when the player has won or lost.

[Github link](https://github.com/06erdem/ChatGPT-Think-Alouds-Supplementary-Materials/).


