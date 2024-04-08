Lisha Qu

Question1:
---
After practicing with Otree, I found it a convenient and flexible application for experimental game theory. However, limitations still exist, and I will explain them from three aspects: 




a) Firstly, oTree's intricate interface has many undefined terms, like parameters that are unfriendly to the green hand, especially for researchers lacking advanced academic expertise. My own experience deploying the trust game revealed the arduous task of configuring instructions and payment mechanisms. A brief explanation of each page's functions and its details and intuitive design features are imperative to overcome this challenge. For example, the tree lacks quick-access guidance on each parameter of the Game. In detail, on the 'trust' part to modify the game theory, it did not explicitly explain the functions of Integers. Having a brief function introduction would be a good choice. 

b) Secondly, oTree neglects essential psychological factors such as emotions and beliefs, which are critical in understanding human decision-making. Behavioral game theory research necessitates tools adaptable to diverse human behaviors. Integrating psychological insights into the software architecture ensures a more comprehensive understanding of strategic interactions. This can be solved by character cosplay in this Game, as players will be assigned to certain beliefs, social statuses, etc.

c) Furthermore, oTree's simplistic assumption of one-time games fails to capture the complexities of real-world interactions characterized by repeated engagements and learning from past experiences. My attempt to model repeated trust games using Otree felt restrictive. An advanced solution must accommodate long-term relationships, reputations, and learning dynamics inherent in strategic interactions. Also, stimulative awards should be added, like some priorities in game theory.

'Game theory: Playing with Behavior: Game Theory and Behavioral Modeling，' March 2, 2024. Game Theory: Playing with Behavior: Game Theory and Behavioral Modeling - FasterCapital



Question 2 
---

1. Limitations of Current MARL Frameworks:

 Environment Constraints: Existing MARL frameworks may struggle with the dynamic and unpredictable nature of the 2048 game environment. The ample state space and complex interactions between tiles present challenges for agents to navigate effectively.

 Agent Algorithm Customizations: Current MARL frameworks lack the flexibility to customize agent algorithms to adapt to the evolving game state and player strategies in 2048. This can limit the agents' ability to learn optimal policies for achieving high scores. The only two parameters is max_itera, which is the maximum time of creating a new blocks, without fulfilling the total grids.



2. Features of MARL Agent for 2048:

 Defining States: In 2048, states are represented by the configuration of the game board, including the values of the last tiles. Additional state features include the actions the system chose last time. The state is limited to 0 to 3, which corresponds to four directions. 

 Actions: Actions correspond to the player's moves, such as merging tiles in different directions (up, down, left, right). Agents choose actions based on their current state and learned strategies, aiming to maximize their score by combining tiles and achieving higher-valued tiles.

 Rewards: Rewards are based on the outcome of each move, with higher rewards for merging higher-valued tiles and achieving higher scores. Additionally, rewards may penalize inefficient moves or premature game endings to encourage agents to learn optimal long-term strategies.

3. Overcoming MARL Limitations:

 Environment Flexibility: Advanced MARL frameworks should offer more flexible environment setups, allowing agents to learn and adapt to the dynamic nature of 2048 gameplay. This flexibility enables agents to explore diverse strategies for combining tiles and achieving high scores. For example, it can create an interactive user-system platform in which users decide the movements.

 Algorithm Customizations: Enhanced algorithm customizations empower agents to develop more sophisticated strategies for playing 2048. For example, agents could employ strategic planning techniques to anticipate future tile placements and optimize their moves accordingly. Additionally, agents could learn from human gameplay data to incorporate expert strategies into their decision-making process. Imagine an advanced MARL framework for playing 2048 where agents are trained using deep reinforcement learning algorithms such as Deep Q-Networks (DQN) or Proximal Policy Optimization (PPO). These agents interact with the game environment and learn from their experiences to improve their gameplay over time.

In this framework, agents learn to recognize patterns in the game board and develop strategies for combining tiles efficiently. They learn to prioritize certain moves over others based on their potential to create high-valued tiles and achieve higher scores.



Question 3 Brainstorm your research idea by criticizing existing research: 
---

1. Summary of the Paper

Core Research Questions: A) How can partial clients be utilized to let the data unbiasedly converge? B) How do you measure clients' contributions and design money awards?

• Methodologies: 

The method is a computer experiment to mimic the situation. 

To achieve this, they propose a game-theoretic-Stackelberg Game approach with randomized client participation and customized pricing strategies. The methodology involves modeling the interaction between the server and clients as a two-stage Stackelberg game, where the server leads in pricing decisions, and clients respond by selecting participation levels. This approach aims to minimize budget usage while evaluating participants' contributions and data relevance.

• Application Scenarios: 

Application scenarios primarily focus on FL environments, particularly in mobile edge networks, where the proposed mechanism could incentivize client participation effectively. By leveraging game theory and adaptive model aggregation, the paper offers insights into optimizing incentive structures and managing economic constraints in FL scenarios across various sectors such as healthcare, mobile device networks, and financial services.

2. Critique of the Research Question

In terms of the research question, the first is how to minimize the cost of FL, both in data communication (model parameters) and how to use a more efficient algorithm to converge quickly. Also, it's vital to figure out the evaluation for the client distribution. Because for the game-theoretic-Stackelberg Game, the utility function is vital and greatly affects followers' reaction to leaders.

3. Critique of the Methodology

The responses raise valid concerns about the assumptions made in the paper regarding participant behavior and incentive mechanisms. The paper assumes rational behavior among participants, expecting them to respond predictably to incentives. However, as mentioned in the meeting discussion, participants may exploit the system by initially providing high-quality data but then uploading noise in subsequent rounds, making it difficult to detect outliers. This raises questions about the effectiveness of the proposed incentive mechanism and the realism of assuming entirely rational behavior among participants.

4. Critique of the Application Scenario

The responses raise valid points about the limitations and uncertainties surrounding the presented federated learning scenarios. The "egg and chicken" problem highlighted by Professor Luo underscores a fundamental challenge in defining participants' intrinsic value without access to their datasets, presenting a significant barrier to implementing effective incentive mechanisms. Moreover, the lack of empirical validation with real-world users calls into question the feasibility and scalability of the proposed approach in practical scenarios.

In light of the rapid advancements in technology, Blockchain technology, for example, offers the potential to enhance the transparency and security of federated learning processes by providing an immutable ledger for tracking model updates and participant contributions. Integrating generative AI models within the federated learning framework could address data scarcity and privacy concerns by synthesizing realistic datasets for training models.

5. Beyond Computer Science and Economics


Bibliography:
---
'Game theory: Playing with Behavior: Game Theory and Behavioral Modeling，' March 2, 2024. https://fastercapital.com/topics/limitations-and-criticisms-of-game-theory-in-behavioral-modeling.html 
