| Term | Description |
| - | - |
| <a id="action-value-function"></a>Action-value function | For each state and action pair, the action-value function outputs the expected reutrn if the agent <b>starts at that state, takes an action</b>, and then follows the policy forever after. |  
| <a id="agent"></a>Agent | To make intelligent decisions, learns from the [environment](#environment) by interacting with it through trial and error and receiving [rewards](#reward) (positive or negative) as unique feedback. | 
| Bellman equation | Instead of calculating each value as the sum of the expected return, <b>which is a long process</b>, we calculate the value as the <b>sum of immediate reward + the discounted value of the state that follows<b>. |
| Continuous taskss | Tasks that has a starting point, but no ending point. |
| <a id="cumulative-reward"> Cumulative reward | Sum of all rewards in a sequence. |
| Deep RL | Introduced deep neural networks to [RL](#RL) problems, hence the name "deep". |
| <a id="discount"></a>Discount | Performed because rewards obtained at the start are more likely to happen as they are more predictable than long-term rewards. <br> - Smaller discount (larger gamma) ⇒ Agent cares more about long-term reward. <br> - Larger discount (smaller gamma) ⇒ Agent cares more about short-term reward. |
| <a id="environment"></a>Environment | Simulated world where an <b>agent can learn by interacting with it</b>. |
| <a id="episodic-tasks"></a>Episodic tasks | Has a starting point and an ending point. |
| Greedy policy |  | 
| Learning strategies | <b>Strategies on how to train our value function or policy function</b>. <b>Uses  experience to solve the RL problem. </b><br> Two learning strategies:<br> - Monte-Carlo<br> - Temporal Difference |
|Monte Carlo Learning | Uses <b>an entire episode of experience before learning</b>  (i.e., update the value function). |
| <a id="policy"></a>Policy | <b>Agent's brain (or) decision-making process</b>. Tells the agent what action to take, given a state.<br>Two types: [Policy-based](#policy-based), [Value-based](#value-based) |
| <a id="policy-based"></a>Policy-based methods | Trains a policy directly to <b>learn which action to take given a state</b>. <br> - Input: State <br>- Output: Action to take at that state. <br>Two types: Deterministic, Stochastic.| 
| <a id="reward"></a>Reward | Fundamental factor in RL. Tells agent whether the action taken is good/bad. |
| Reward hypothesis | [RL](#RL) problems can be formulated as a maximization of the (cumulative) reward | 
| <a id="RL"></a>RL |  Build [agents](#agent) that can make smart decisions. <br>RL algorithms are focused on <b>maximizing the [cumulative reward](#cumulative-reward)</b>. <br> Goal of an RL is to have an optimal policy π.| 
| <a id="state-value-function"></a>State-value function | For each state, the state-value function outputs the exepcted return if the agent <b>starts at that state</b> and then follows the policy forever after.|
| Temporal Difference Learning| Uses <b>only a step (one interaction) to learn</b> (i.e., update the value function), |  
|  <a id="value-based"></a>Value-based methods | Trains a value function to <b>learn which states are more valuable</b> and use this value function to <b>take action that leads to it</b>. <br><br><b>Two value based algos</b>: <br> - Q-Learning, <br> - Deep Q-Learning. <br><br> <b>Two types of value based functions</b>:<br>- [State value function](#state-value-function): Calculates value of a state.<br> - [Action value function](#action-value-function): Calculates value of state-action pair. |
| | |