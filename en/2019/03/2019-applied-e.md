---
title: "2019 Applied Ethical and Governance Challenges in AI - Notes from Part 1: Diagnosis"
date: 2019-03-07T00:00:00
permalink: https://joi.ito.com/weblog/2019/03/07/2019-applied-et.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2019/03/07/2019-applied-et.html
extracted: 2025-12-25
---

Jonathan Zittrain and I are co-teaching a class together for the third time. This year, the title of the course is Applied Ethical and Governance Challenges in Artificial Intelligence. It is a seminar, which means that we invite speakers for most of the classes and usually talk about their papers and their work. The speakers and the papers were mostly curated by our amazing teaching assistant team - Samantha Bates, John Bowers and Natalie Satiel.

One of the things that Sam does is help prepare for the class by summarizing the paper and the flow of the class and I realized that it was a waste for this work to just be crib notes for the instructors. I asked Sam for permission to publish the notes and the syllabus on my blog as a way for people to learn some of what we are learning and start potentially interesting conversations.

The course is structured as three sets of three classes on three focus areas. Previous classes were more general overviews of the space, but as the area of research matured, we realized that it would be more interesting to go deep in key areas than to go over what a lot of people probably already know.

We chose three main topics: fairness, interpretability, and adversarial examples. We then organized the classes to hit each topic three times, starting with diagnosis (identifying the technical root of the problem), then prognosis (exploring the social impact of those problems) then intervention (considering potential solutions to the problems we've identified while taking into account the costs and benefits of each proposed solution). See the diagram below for a visual of the structure.

The students in the class are half MIT and half Harvard students with diverse areas of expertise including software engineering, law, policy and other fields. The class has really been great and I feel that we're going deeper on many of the topics than I've ever gone before. The downside is that we are beginning to see how difficult the problems are. Personally, I'm feeling a bit overwhelmed by the scale of the work we have ahead of us to try to minimize the harm to society by the deployment of these algorithms.

We just finished the prognosis phase and are about to start intervention. I hope that we find something to be optimistic about as we enter that phase.

Please find below the summary and the syllabus for the introduction and the first phase - the diagnosis phase - by Samantha Bates along with links to the papers.

The tl;dr summary of the first phase is... we have no idea how to define fairness and it probably isn't reducible to a formula or a law, but it is dynamic. Interpretability sounds like a cool word, but as Zachary Lipton said in his talk to our class, it is a "wastebasket taxon" like the word "antelope" where we call anything that sort of looks like an antelope, an antelope, even if it has really no relationship with other antelopes. A bunch of students from MIT made it very clear to us that we are not prepared for adversarial attacks and that it was unclear whether we could build algorithms that were both robust against these attacks and still functionally effective.

**Part 1: Introduction and Diagnosis**

*By Samantha Bates*

![](https://lh3.googleusercontent.com/mbxEwNyXALP8zp3eT85A1SAkUzbzNL28CGygZ1S6yoYxBhSclO-PpX4kID5j0mapz2efUy4EOl_g5uTJtbg-ISe5QiV5KWmlug-reMn1jSAW4pyievAPG0CtNXISIrsj--Dv75PB)

***Syllabus Notes: Introduction and Diagnosis Stage***

This first post summarizes the readings assigned for the first four classes, which encompasses the introduction and the diagnosis stage. In the diagnosis stage, the class identified the core problems in AI related to fairness, interpretability, and adversarial examples and considered how the underlying mechanisms of autonomous systems contributed to those problems. As a result, our class discussions involved defining terminology and studying how the technology works. Included below is the first part of the course syllabus along with notes summarizing the main takeaways from each of the assigned readings.

**Class Session 1: Introduction**

In our first class session, we presented the structure and motivations behind the course, and set the stage for later class discussions by assigning readings that critique the current state of the field.

- "[Artificial Intelligence -- The Revolution Hasn't Happened Yet](https://perma.cc/4JM9-E4HC)" by Michael Jordan, Medium (April 2018)
- "[Troubling Trends in Machine Learning Scholarship](https://perma.cc/H6Q9-HZZD)" by Zachary C. Lipton & Jacob Steinhardt (July 2018)

Both readings challenge the way Artificial Intelligence (AI) research is currently conducted and talked about, but from different perspectives. Michael Jordan's piece is mainly concerned with the need for more collaboration across disciplines in AI research. He argues that we are experiencing the creation of a new branch of engineering that needs to incorporate non-technical as well as engineering challenges and perspectives. "Troubling Trends in Machine Learning Scholarship" focuses more on falling standards and non-rigorous research practices in the academic machine learning community. The authors rightly point out that academic scholarship must be held to the highest standards in order to preserve public and academic trust in the field.

We chose to start out with readings that critique the current state of the field because they encourage students to think critically about the papers they will read throughout the semester. Just as the readings show that the use of precise terminology and explanation of thought are particularly important to prevent confusion, we challenge students to carefully consider how they present their own work and opinions. The readings set the stage for our deep dives into specific topic areas (fairness, interpretability, adversarial AI) and also set some expectations about how students should approach the research we will discuss throughout the course.

**Class Session 2: Diagnosing problems of fairness**

For our first class in the diagnosis stage, the class was joined by Cathy O'Neil, a data scientist and activist who has become one of the leading voices on fairness in machine learning.

- Weapons of Math Destruction by Cathy O'Neil, Broadway Books (2016). Read Introduction and Chapter 1: "Bomb Parts: What Is a Model?"
- [OPTIONAL] "[The scored society: due process for automated predictions](https://perma.cc/8QD4-JQAS)" by Danielle Keats Citron and Frank Pasquale, Washington Law Review (2014)

Cathy O'Neil's book, Weapons of Math Destruction, is a great introduction to predictive models, how they work, and how they can become biased. She refers to flawed models that are opaque, scalable, and have the potential to damage lives (frequently the lives of the poor and disadvantaged) as Weapons of Math Destruction (WMDs). She explains that despite good intentions, we are more likely to create WMDs when we don't have enough data to draw reliable conclusions, use proxies to stand in for data we don't have, and try to use simplistic models to understand and predict human behavior, which is much too complicated to accurately model with just a handful of variables. Even worse, most of these algorithms are opaque, so the people impacted by these models are unable to challenge their outputs.

O'Neil demonstrates that the use of these types of models can have serious unforeseen consequences. Because WMDs are a cheap alternative to human review and decision-making, WMDs are more likely to be deployed in poor areas, and thus tend to have a larger impact on the poor and disadvantaged in our society. Additionally, WMDs can actually lead to worse behavior. In O'Neil's example of the Washington D.C. School District's model that used student test scores to identify and root out ineffective teachers, some teachers changed their students' test scores in order to protect their jobs. Although the WMD in this scenario was deployed to improve teacher effectiveness, it actually had the opposite effect by creating an unintended incentive structure.

The optional reading, "The Scored Society: Due Process for Automated Predictions," discusses algorithmic fairness in the credit scoring context. Like Cathy O'Neil, the authors contend that credit scoring algorithms exacerbate existing social inequalities and argue that our legal system has a duty to change that. They propose opening the credit scoring and credit sharing process to public review while also requiring that credit scoring companies educate individuals about how different variables influence their scores. By attacking the opacity problem that Cathy O'Neil identified as one of three characteristics of WMDs, the authors believe the credit scoring system can become more fair without infringing on intellectual property rights or requiring that we abandon the scoring models altogether.

**Class Session 3: Diagnosing problems of interpretability**

Zachary Lipton, an Assistant Professor at Carnegie Mellon University who is working intensively on defining and addressing problems of interpretability in machine learning, joined the class on Day 3 to discuss what it means for a model to be interpretable.

- "[The Mythos of Model Interpretability](https://perma.cc/6MV7-HLHB)" by Zachary C. Lipton, ArXiv (2016)
- [OPTIONAL] "[Towards a rigorous Science of Interpretable Machine Learning](https://perma.cc/U7FF-NPZ5)" by Finale Doshi-Velez and Been Kim, ArXiv (2017)

Class session three was our first day discussing interpretability, so both readings consider how best to define interpretability and why it is important. Lipton's paper asserts that interpretability reflects a number of different ideas and that its current definitions are often too simplistic. His paper primarily raises stage-setting questions: What is interpretability? In what contexts is interpretability most necessary? Does creating a model that is more transparent or can explain its outputs make it interpretable?

Through his examination of these questions, Lipton argues that the definition of interpretability depends on why we want a model to be interpretable. We might demand that a model be interpretable so that we can identify underlying biases and allow those affected by the algorithm to contest its outputs. We may also want an algorithm to be interpretable in order to provide more information to the humans involved in the decision, to give the algorithm more legitimacy, or to uncover possible causal relationships between variables that can then be tested further. By clarifying the different circumstances in which we demand interpretability, Lipton argues that we can get closer to a working definition of interpretability that better reflects its many facets.

Lipton also considers two types of proposals to improve interpretability: increasing transparency and providing post-hoc explanations. The increasing transparency approach can apply to the entire model (simulatability), meaning that a user should be able to reproduce the model's output if given the same input data and parameters. We can also improve transparency by making the different elements of the model (the input data, parameters, and calculations) individually interpretable, or by showing that during the training stage, the model will come to a unique solution regardless of the training dataset. However, as we will discuss further during the interventions stage of the course, providing more transparency at each level does not always make sense depending on the context and the type of model employed (for example a linear model vs. a neural network model). Additionally, improving the transparency of a model may decrease the model's accuracy and effectiveness. A second way to improve interpretability is to require post-hoc interpretability, meaning that the model must explain its decision-making process after generating an output. Post-hoc explanations can take the form of text, visuals, saliency maps, or analogies that show how a similar decision was reached in a similar context. Although post-hoc explanations can provide insight into how individuals affected by the model can challenge or change its outputs, Lipton cautions that these explanations can be unintentionally misleading, especially if they are influenced by our human biases.

Ultimately, Lipton's paper concludes that it is extremely challenging to define interpretability given how much it depends on external factors like context and the motivations for making a model interpretable. Without a working definition of the term it remains unclear how to determine whether a model is interpretable. While the Lipton paper focuses more on defining interpretability and considering why it is important, the optional reading, "Towards a rigorous Science of Interpretable Machine Learning," dives deeper into the various methods used to determine whether a model is interpretable. The authors define interpretability as the "ability to explain or present in understandable terms to a human" and are particularly concerned about the lack of standards for evaluating interpretability.

**Class Session 4: Diagnosing vulnerabilities to adversarial examples**

In our first session on adversarial examples, the class was joined by [LabSix](https://www.labsix.org/), a student-run AI research group at MIT that is doing cutting-edge work on adversarial techniques. LabSix gave a primer on adversarial examples and presented some of its own work.

- "[Motivating the Rules of the Game for Adversarial Example Research](https://perma.cc/3ZQQ-A7MY)" by Justin Gilmer et al., ArXiv (2018).
- [RECOMMENDED] "[Intriguing properties of neural networks](https://perma.cc/W2FG-CNNC)" by Christian Szegedy et al., ArXiv (2013)

The Gilmer et. al. paper is an accessible introduction to adversarial examples that defines them as "inputs to machine learning models that an attacker has intentionally designed to cause the model to make a mistake." The main thrust of the paper is an examination of the different scenarios in which an attacker may employ adversarial examples. The authors develop a taxonomy to categorize these different types of attacks: "indistinguishable perturbation, content-preserving perturbation, non-suspicious input, content-constrained input, and unconstrained input." For each category of attack, the authors explore the different motivations and constraints of the attacker. By gaining a better understanding of the different types of attacks and the tradeoffs of each type, the authors argue that the designers of machine learning systems will be better able to defend against them.

The paper also includes an overview of the perturbation defense literature, which the authors criticize for failing to consider adversarial example attacks in plausible, real-world situations. For example, a common hypothetical situation posed in the defense literature is an attacker perturbing the image of a stop sign in an attempt to confuse a self-driving car. The Gilmer et. al. paper; however, points out that the engineers of the car would have considered and prepared for naturally occurring misclassification errors caused by the system itself or real world events (for example, the stop sign could be blown over by the wind). The authors also argue that there are likely easier, non technical methods that the attackers could use to confuse the car, so the hypothetical is not the most realistic test case. The authors' other main critique of the defense literature is that it does not acknowledge how improving certain aspects of a system's defense structure can make other aspects of the system less robust and thus more vulnerable to attack.

The recommended reading by Christian Szegedy et. al. is much more technical and requires some machine learning background to understand all of the terminology. Although it is a challenging read, we included it in the syllabus because it introduced the term "adversarial examples" and laid some of the foundation for research on this topic.

###### Credits

Figure and Notes by Samantha Bates

Syllabus by Samantha Bates, John Bowers and Natalie Saltiel