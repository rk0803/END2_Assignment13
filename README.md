# Assignment 13
This assignment is based on the transformer model, developed from scratch, as in paper, "Attention is all you need".</br>
The Transformer architecure is not based on recurrence, instead the model is entirely made up of linear layers, attention mechanisms and normalization.
Of latemTransformers have been purported as most effective models used in various NLP tasks to achieve state-of-the-art results. 

In this implementation, a learned positional encoding used instead of a static one mentioned in the paper. A standard Adam optimizer with a static learning rate is used. The Model is to be trained on Multi30k dataset, for German to English translation, without using the legacy stuff.

## Training log
Model was trained for 20 epochs. Training starts with very high training and valid perplexity, which steadily reduces. Training perplexity reduces faster than the vaild perplexity. Here is the taining log for last 5 epochs.
Epoch| Train Loss | Train Perplexity | Valid Loss | Valid Perplexity |
----------|--------|-----------|----------|----------- |
Epoch: 15 |  1.799 |  6.044 | 2.592 |   13.356
Epoch: 16 |  1.675 |  5.339 | 	2.560 |   12.930
Epoch: 17 | 1.556 |  4.738 |	2.526 |   12.505
Epoch: 18 | 1.446 |  4.247 |	 2.530 |   12.558
Epoch: 19 |  1.345 |   3.839 |	 2.525 |    12.495
Epoch: 20 |  1.242 |   3.461 |	 2.547 |   12.772

## Predicted Translations (after 20 epochs)
A look at some 10 German sentences, along with their original English translation and as predicted by the model are listed below:
Sr. No. | German | Original English Translation  | Translation as predicted by the Model |
--------|--------|-------------------------------|---------------------------------------|
1 | Ein Mann mit einem orangefarbenen Hut, der etwas anstarrt.| A man in an orange hat starring at something. | A man in a orange hat is using his drill . <eos> |
2 | Ein Boston Terrier läuft über saftig-grünes Gras vor einem weißen Zaun. |A Boston Terrier is running on lush green grass in front of a white fence.| A husky eastern greyhound dogs are running through the grass  . <eos> |
3 | Ein Mädchen in einem Karateanzug bricht einen Stock mit einem Tritt. | A girl in karate uniform breaking a stick with a front kick.|A girl in a karate uniform is wearing a helmet and is wearing a stick . <eos> |
4 | Fünf Leute in Winterjacken und mit Helmen stehen im Schnee mit Schneemobilen im Hintergrund. |  Five people wearing winter jackets and helmets stand in the snow, with snowmobiles in the background. | Five people in different colored uniforms and helmets are standing in the snow with a shovel in the background . <eos> |
5 | Leute Reparieren das Dach eines Hauses. | People are fixing the roof of a house.| People are cleaning the roof of a house . <eos> |
6 | Ein hell gekleideter Mann fotografiert eine Gruppe von Männern in dunklen Anzügen und mit Hüten, die um eine Frau in einem trägerlosen Kleid herum stehen.  | A man in light colored clothing photographs a group of men wearing dark suits and hats standing around a woman dressed in a strapless gown. | A man in a dark suit , and a woman in a dark suit , is dancing in a dark room with a woman in a dark - sleeved t - style dress and a woman in a woman in a woman in a woman in a woman in a |
7 | Eine Gruppe von Menschen steht vor einem Iglu. | A group of people standing in front of an igloo. | A group of people standing in front of an airport . <eos> |
8 | Ein Junge in einem roten Trikot versucht, die Home Base zu erreichen, während der Catcher im blauen Trikot versucht, ihn zu fangen. | A boy in a red uniform is attempting to avoid getting out at home plate, while the catcher in the blue uniform is attempting to catch him.  |  A boy in a red uniform tries to catch a red ball from a rodeo , as the middle of a blue uniform tries to block his red ball in a rodeo , a boy in blue uniform , a basketball player in a basketball player in a basketball player |
9 | Ein Typ arbeitet an einem Gebäude. | A guy works on a building. | A guy working on a building . <eos> |
10 | Ein Mann in einer Weste sitzt auf einem Stuhl und hält Magazine. | A man in a vest is sitting in a chair and holding magazines.  |  A man in a vest is sitting in a chair holding a spoon . <eos> |
  
  
### Team Members
  Ritambhra Korpal </br>
  Pralay Ramteke </br>
  Chaitnaya Vanapamala </br>
  Pallavi
  
