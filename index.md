# Replication Package for CoLiCo
<!-- ## Replication Package for Our Paper: Beyond Literal Meaning: Uncover and Explain Implicit Knowledge in Code through Wikipedia-based Concept Linking -->

In this replication package, we show the evaluation data and results of CoLiCo (i.e., Concept Linking for Code). To evaluate the quality, accuracy, significance and usefulness of CoLiCo, we conduct a series of experimental studies which answer the following research questions.

- **RQ1 (Accuracy):** How accurate are the concept linkings and explanations uncovered by CoLiCo? Can it outperform existing word sense disambiguation and entity linking approaches for general text?
- **RQ2 (Significance):** How significantly do the mentions of Wikipedia concepts in reusable source code affect the program comprehension?
- **RQ3 (Usefulness):** Can the linked concepts and extracted explanations help developers comprehend the implicit knowledge behind code?

We use the code snippets in the adaptation dataset constructed by Zhang et al. Their purpose was to study the reuse and adaptation of the code snippets on Stack Overflow and the code snippets were identified by linking code snippets on Stack Overflow to their counterparts in GitHub repositories. The dataset includes 629 Java code snippets and each of them is a method with 32.7 lines of code on average. We choose this dataset as these code snippets have been widely reused and adapted and the reuse and adaptation are based on in-depth comprehension of the code.

## RQ1
To evaluate the accuracy of CoLiCo’s online linking, we randomly select 50 code snippets that are included in different Stack Overflow posts from the adap tation dataset. These code snippets cover different domains such as encryption, network, image, GUI. We use CoLiCo to identify Wikipedia concept linkings and explanations for the 50 code snippets. We choose a word sense disambiguation and entity linking approach called Babelfy as the baseline. The evaluation results are as follows:

Concept Linking by CoLiCo
Explanantion Excerption by CoLiCo
Concept Linking by Babelfy

## RQ2
We use two metrics to evaluate the significance of the concept linkings, i.e., ease and importance. A concept linking is considered significant if it is both difficult (i.e., at least 3 of the 4 annotators somewhat agree or agree) and important (i.e., at least 3 of the 4 annotators somewhat agree or agree).

The evaluation results of significance as follows:
Significance

## RQ3
We use 5 reading and comprehension tasks with 13 questions to evaluate the usefulness of CoLiCo, the tasks and questions are as follows:

Reading and Comprehension Tasks

## Video Demo
This is a video demo for CoLiCo: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/OJjuUD5aGaI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

