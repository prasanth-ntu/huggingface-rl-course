| Term | Description |
| - | - |
| <a id="action-value-function"></a>Action-value function | For each state and action pair, the action-value function outputs the expected reutrn if the agent <b>starts at that state, takes an action</b>, and then follows the policy forever after. |  
| <a id="agent"></a>Agent | To make intelligent decisions, learns from the [environment](#environment) by interacting with it through trial and error and receiving [rewards](#reward) (positive or negative) as unique feedback. | 
| Bellman equation | Instead of calculating each value as the sum of the expected return, <b>which is a long process</b>, we calculate the value as the <b>sum of immediate reward + the discounted value of the state that follows<b>. |
| Continuous taskss | Tasks that has a starting point, but no ending point. |
| <a id="cumulative-reward"> Cumulative reward | Sum of all rewards in a sequence. |
| Deep Q Algorithm |  |
| <a id="deep-q-learning"></a>Deep Q-Learning | Instead of using a [Q-table](#q-table), deep Q-learning uses a Neural Network that takes a state and approximates Q-valuse  for each action based on that state. |
| Deep RL | Introduced deep neural networks to [RL](#RL) problems, hence the name "deep". |
| <a id="discount"></a>Discount | Performed because rewards obtained at the start are more likely to happen as they are more predictable than long-term rewards. <br> - Smaller discount (larger gamma) ⇒ Agent cares more about long-term reward. <br> - Larger discount (smaller gamma) ⇒ Agent cares more about short-term reward. |
| <a id="environment"></a>Environment | Simulated world where an <b>agent can learn by interacting with it</b>. |
| <a id="episodic-tasks"></a>Episodic tasks | Has a starting point and an ending point. |
| <a id="epsilon-greedy-policy"></a>Epsilon-greedy policy | Policy that handles the exploration/exploitation trade-off. <br> Epsilon is typically decreased over time (training) to shift focus from exploration to exploitation. | 
| <a id="exploitation"></a>Exploitation | |
| <a id="exploration"></a>Exploration | |
| Greedy policy | Policy where the agent always chooses the action with the highest estimated reward, based on the current knowledge of the environment (=> Only [exploitation](#exploitation), and no [exploration](#exploration)). While this policy may seem optimal, it often isn't, because the agent may get stuck in a local maximum and stop exploring potentially higher-reward actions.  <br> Variants: <br>- [Epsilon-greedy policy](#epsilon-greedy-policy) | 
| Learning strategies | <b>Strategies on how to train our value function or policy function</b>. <b>Uses  experience to solve the RL problem. </b><br> Two learning strategies:<br> - Monte-Carlo<br> - Temporal Difference |
| <a id="monte-carlo-learning"></a>Monte Carlo (MC) Learning | Uses <b>an entire episode of experience before learning</b>  (i.e., update the value function or policy function). |
| <a id="off-policy"></a>Off-policy | Using <b>a different policy for acting (inference) and updating (training)</b>. <br> Example: [Q-learning](#q-learning). |
| <a id="on-policy"></a>On-policy | Using the <b>same policy for acting (inference) and updating (training)</b>. <br>Example: SARSA learning.|
| <a id="policy"></a>Policy | <b>Agent's brain (or) decision-making process</b>. Tells the agent what action to take, given a state.<br>Two types: [Policy-based](#policy-based), [Value-based](#value-based) |
| <a id="policy-based"></a>Policy-based methods | Trains a policy directly to <b>learn which action to take given a state</b>. <br> - Input: State <br>- Output: Action to take at that state. <br>Two types: Deterministic, Stochastic.| 
| <a id="q-function"></a>Q-Function | An <b>[action-value function](#action-value-function)</b> that determines the value of being at a particular state and taking a specific action at that state. <br> Q-function is encoded by a [Q-table](#q-table). Given a state and a function, Q-function will search its Q-table for the corresponding value. <br> The <b>Q comes from the "Quality" of that action at that state.</b> |
| <a id="q-learning"></a>Q-Learning |<b>[Off-policy](#off-policy) value-based method that uses a [TD](#temporal-difference-learning) approach to train its [action-value function](#action-value-funciton)</b>.<br> An <b>RL algorithm we use to train [Q-function](#q-function).</b><br><br> Works well with small state space environments like `FrozenLake` (16 states), `Taxi-v3` (500 states). However, it's not scalable for states and action spaces that are not small enough. For such cases, we have to use [Deep Q-Learning](#deep-q-learning). | 
| <a id="q-table"></a>Q-Table | A <b>table where each cell corresponds to state-action pair</b>. Think of it like a <b>memory or a cheat-sheet of our [Q-function](#q-function)</b>. | 
| <a id="reward"></a>Reward | Fundamental factor in RL. Tells agent whether the action taken is good/bad. <b>It's the feedback we get from the environment</b> after performing an action at a state. |
| Reward hypothesis | [RL](#RL) problems can be formulated as a maximization of the (cumulative) reward | 
| <a id="RL"></a>RL |  Build [agents](#agent) that can make smart decisions. <br>RL algorithms are focused on <b>maximizing the [cumulative reward](#cumulative-reward)</b>. <br> Goal of an RL is to have an optimal policy π.| 
| <a id="state-value-function"></a>State-value function | For each state, the state-value function outputs the exepcted return if the agent <b>starts at that state</b> and then follows the policy forever after.|
| <a id="temporal-difference-learning"></a>Temporal Difference (TD) Learning| Uses <b>only a step (one interaction) to learn</b> (i.e., update the value function), instead of entire episode like [Monte Carlo learning](#monte-carlo-learning) |  
| Value of a state or a state-action pair| Expected cumulative [reward](#reward) agent gets if it starts at this state (or state-action pair) nad then acts accordingly to its policy. |
|  <a id="value-based"></a>Value-based methods | Trains a value function to <b>learn which states are more valuable</b> and use this value function to <b>take action that leads to it</b>. <br><br><b>Two value based algos</b>: <br> - Q-Learning, <br> - Deep Q-Learning. <br><br> <b>Two main types (strategies) of value based functions</b>:<br>- [State value function](#state-value-function): Calculates value of a state.<br> - [Action value function](#action-value-function): Calculates value of state-action pair. |
| | |