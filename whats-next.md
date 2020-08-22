---
description: The Next in the field of Causal Inference
---

# What's Next

## **Causality in Vision domain:**

Currently, the image analysis is mainly based on pixel information, but we can build a causal structure that can help in understanding the images better. If you wanted a neural network to detect when people are dancing, you’d show it many, many images of dancers. If you wanted it to identify when people are running, you’d show it many, many images of runners. The system would learn to distinguish runners from dancers by **identifying features that tend to be different in the images**, such as the positions of a person’s hands and arms. But **Bengio** points out that fundamental knowledge about the world can be gleaned by analyzing the things that are similar or “invariant” across data sets. Maybe a neural network could learn that movements of the legs physically cause both running and dancing. Maybe after seeing these examples and many others that show people only a few feet off the ground, a machine would eventually understand something about gravity and how it limits human movement. Over time, with enough meta-learning about variables that are consistent across data sets, a computer could gain causal knowledge that would be reusable in many domains. - [MIT Review](https://www.technologyreview.com/2020/02/19/868178/what-ai-still-cant-do/)

## **CausalRL:**

Causal Reinforcement Learning = Causal Inference + Reinforcement Learning

It is a process where the Causal Models tries to explicitly define the causal relationships of the real-world environment, and RL is used for optimizing the policy based on this predefined causal Model.

RL is mostly used in the Gaming industry today, where the causal structure is pre-defined. Humans have built the games so we actually know the structure of the world we have built, hence we have the causal structure for this game-world. In the case of the real-world, we do not have the causal structure\(at least till date\). When we implement this technique of Reinforcement learning to optimize the output by running multiple scenarios on the real-world causal structure, it could be really helpful.

## **Causality for Robotics:**

For building human-like robots we have to equip machines with a model of the environment. If a machine does not have a model of reality, we cannot expect that the machine will behave intelligently in that reality. We would have to conceptualize models and program the reality into a model.

The next step will be that machines will postulate such models on their own and will verify and refine them based on empirical evidence. That is what happened to science, we started with a geocentric model, with circles and epicycles, and ended up with a heliocentric model with its ellipses. Robots, too, will communicate with each other and will translate this hypothetical world, this wild world, of metaphorical models.

