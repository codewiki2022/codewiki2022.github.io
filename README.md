<!-- # Replication Package of CoLiCo -->

In this replication package, we show the evaluation data and results of CoLiCo (i.e., **Co**ncept **Li**nking for **Co**de).
To evaluate the accuracy, significance and usefulness of CoLiCo, we conduct a series of experimental studies which answer the following research questions.
- **RQ1 (Accuracy):** How accurate are the concept linkings and explanations uncovered by CoLiCo? Can it outperform existing word sense disambiguation and entity linking approaches for general text?
- **RQ2 (Significance):** How significantly do the mentions of Wikipedia concepts in reusable source code affect the program comprehension?
- **RQ3 (Usefulness):** Can the linked concepts and extracted explanations help developers comprehend the implicit knowledge behind code?

We use the code snippets in the [*adaptation*](https://figshare.com/articles/dataset/ICSE_artifact/7722068/2?file=14372909) dataset constructed by Zhang et al.
Their purpose was to study the reuse and adaptation of the code snippets on Stack Overflow and the code snippets were identified by linking code snippets on Stack Overflow to their counterparts in GitHub repositories.
The dataset includes 629 Java code snippets and each of them is a method with 32.7 lines of code on average.
We choose this dataset as these code snippets have been widely reused and adapted and the reuse and adaptation are based on in-depth comprehension of the code.


### RQ1
To evaluate the accuracy of CoLiCo's online linking, we randomly select 50 code snippets that are included in different Stack Overflow posts from the adap tation dataset. These code snippets cover different domains such as encryption, network, image, GUI.
We use CoLiCo to identify Wikipedia concept linkings and explanations for the 50 code snippets. We choose a word sense disambiguation and entity linking approach called Babelfy as the baseline.
The evaluation results are as follows:<br>
- [Concept Linking by CoLiCo](./RQ1_CoLiCo_concept_linking_result.zip)
- [Explanantion Excerption by CoLiCo](./RQ1_CoLiCo_explanation_excerption_result.zip)
- [Concept Linking by Babelfy](./RQ1_Babelfy_concept_linking_result.zip)

### RQ2
We use two metrics to evaluate the significance of the concept linkings, i.e., ease and importance.  A concept linking is considered significant if it is both difficult (i.e., average ease ≤ 2) and important (i.e., average importance ≥ 3). 

The evaluation results of significance as follows:<br>
- [Significance](./RQ2_CoLiCo_significance_result.zip)

### RQ3
We use 5 reading and comprehension tasks with 13 questions to evaluate the usefulness of CoLiCo, the tasks and questions are as follows:<br>
- [Reading and Comprehension Tasks](./RQ3_Tasks.md)


### Video Demo
This is a video demo for CoLiCo: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/OJjuUD5aGaI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>