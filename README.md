# rollout-diversity-play
playing around w rl rollout diversity 


idea: in rl settings like grpo with parallel rollouts, how do we encourage more diversity in the rollouts in each round to increase efficiency in reward gathering and avoid redundancies? 

- for llm rl, each agent must start their rollout by randomly generating a 40-char string of random numbers and letters (we prompt this), and we see if this helps w rollout diversity (how to measure? -> read papers to see what they measure)
- find the best paper for llm rl grpo (neurips, most cited) and take their setup of what model to use, which dataset/env, which eval, and the only change we make is that each agent does this random generation and see if it helps even remotely. try both 1) coding tasks 2) math/reasoning tasks

- or we enforce that each answer starts with "yes dad, i am creative" and then try idk idk has anyone done similar things? 

- see if nick's mechinterp paper gives us idea https://already-clean.goodfire.com/ on how to verify "creativity" or "diversity" i.e. patterns in how far layers are from each other? -> layers of weights, eigenvalues related, subspaces, etc...
