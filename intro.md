# Transfer Learning

In **transfer learning**, experience with one learning task helps an agent learn better on another task. Let's think about the real world, a student who has already learned a programming language finds it easier to learn another one.

It is still not clear the mechanism of humans transfer learning. For neural networks, learning consist of adjusting weigths, so the most plausible approach for transfer learning is to clone the weights learned for task A to a network that will be trained for task B.

Suppose you have to build a natural language system. It is common to start with a pretrained model, wich already "knows" vocabulary and syntax of language. The next step is to fine-tune the model by training on the task it is to perform.
While training, you will want to freeze the layers of the pretreined model, these layers serve as feature detectors that will be useful for the new model. New data will be allowed to modify the weights of the higher level only. These are the layers that identify problem-specific features and do classification.

```{tableofcontents}
```
