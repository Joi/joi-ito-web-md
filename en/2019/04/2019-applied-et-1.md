---
title: "2019 Applied Ethical and Governance Challenges in AI - Notes from Part 3: Intervention"
date: 2019-04-28T00:00:00
permalink: https://joi.ito.com/weblog/2019/04/28/2019-applied-et-1.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2019/04/28/2019-applied-et-1.html
extracted: 2025-12-25
---

**Applied Ethical and Governance Challenges in Artificial Intelligence (AI)**

**Part 3: Intervention**

We recently completed the third and final section of our course that I co-taught with Jonathan Zittrain and TA'ed by Samantha Bates, John Bowers and Natalie Saltiel. The plan was to try to bring the discussion of diagnosis and prognosis in for a landing and figure out how to intervene.

The first class of this section (the eighth class of the course) looked at the use of algorithms in decision making. One paper that we read was the most recent in a series of papers by Jon Kleinberg, Sendhil Mullainathan and Cass Sunstein that supported the use of algorithms in decision making such as pretrial risk assessments - the particular paper we read focused on the use of algorithms for measuring the bias of the decision making. Sendhil Mullainathan, one of the authors of the paper joined us in the class. The second paper was by Rodrigo Ochigame, a history and science and technology in society (STS) student who criticized the fundamental premise of reducing notions such as "fairness" to "computationals formalisms" such as algorithms. The discussion which at points took the form of a lively debate was extremely interesting and helped us and the students see how important it is to question the framing of the questions and the assumptions that we often make when we begin working on a solution without coming to a societal agreement of the problem.

In the case of pretrial risk assessments, the basic question about whether rearrests are more of an indicator of policing practice or the "criminality of the individual" fundamentally changes whether the focus should be on the "fairness" and accuracy of the prediction of the criminality of the individual or whether we should be questioning the entire system of incarceration and its assumptions.

At the end of the class, Sendhil agreed to return to have a deeper and longer conversation with my [Humanizing AI in Law (HAL) team](https://www.media.mit.edu/projects/HAL/people/) to discuss this issue further.

In the next class, we discussed the history of causal inference and how statistics and correlation have dominated modern machine learning and data analysis. We discussed the difficulties and challenges in validating causal claims but also the importance of causal claims. In particular, we looked at how legal precedent has from time to time made references to the right to individualized sentencing. Clearly, risk scores used in sentencing that are protected by trade secrets and confidentiality agreements challenge the right to due process as expressed in the [*Wisconsin v. Loomis*](https://harvardlawreview.org/2017/03/state-v-loomis/) case as well as the right to an individualized sentence.

The last class focused on adversarial examples and technical debt - which helped us think about when and how policies and important "tests" and controls can and should be put in place vs when, if ever, we should just "move quickly and break things." I'm not sure if it was the consensus of the class, but I felt that somehow we needed a new design process that allowed for the creation of design stories and "tests" that could be developed by the users and members of the affected communities that were integrated into the development process - participant design that was deeply integrated into something that looked like agile development story and test development processes. Fairness and other contextual parameters are dynamic and can only be managed through interactions with the systems in which the algorithms are deployed. Figuring out a way to somehow integrate the dynamic nature of the social system seems like a possible approach for mitigating a category of technical debt and designing systems untethered from the normative environments in which they are deployed.

Throughout the course, I observed students learning from one another, rethinking their own assumptions, and collaborating on projects outside of class. We may not have figured out how to eliminate algorithmic bias or come up with a satisfactory definition of what makes an autonomous system interpretable, but we did find ourselves having conversations and coming to new points of view that I don't think would have happened otherwise.

It is clear that integrating humanities and social science into the conversation about law, economics and technology is required for us to navigate ourselves out of the mess that we've created and to chart a way forward into a our uncertain future with our increasingly algorithmic societal systems.

- Joi

**Syllabus Notes**

*By Samantha Bates*

In our final stage of the course, the intervention stage, we investigated potential solutions to the problems we identified earlier in the course. Class discussions included consideration of the various tradeoffs of implementing potential solutions and places to intervene in different systems. We also investigated the balance between waiting to address potential weaknesses in a given system until after deployment versus proactively correcting deficiencies before deploying the autonomous system.

**Class Session 8: Intervening on behalf of fairness**

This class was structured as a conversation involving two guests, University of Chicago Booth School of Business Professor Sendhil Mullainathan and MIT PhD student Rodrigo Ochigame. As a class we debated whether elements of the two papers were reconcilable given their seemingly opposite viewpoints.

- ["Discrimination in the Age of Algorithms"](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3329669&download=yes) by Jon Kleinberg, Jens Ludwig, Sendhil Mullainathan, and Cass R. Sunstein (February 2019).
- [FORTHCOMING] "The Illusion of Algorithmic Fairness" by Rodrigo Ochigame (2019)

The main argument in "Discrimination in the Age of Algorithms" is that algorithms make it easier to identify and prevent discrimination. The authors point out that current obstacles to proving discrimination are primarily caused by opacity around human decision making. Human decision makers can make up justifications for their decisions after the fact or may be influenced by bias without even knowing it. The authors argue that by making algorithms transparent, primarily through the use of counterfactuals, we can determine which components of the algorithm are causing a biased outcome. The paper also suggests that we allow algorithms to consider personal attributes such as race and gender in certain contexts because doing so could help counteract human bias. For example, if managers consistently give higher performance ratings to male workers over female workers, the algorithm won't be able to figure out that managers are discriminating against women in the workplace if it can't incorporate data about gender. But if we allow the algorithm to be aware of gender when calculating work productivity, it may be able to uncover existing biases and prevent them from being perpetuated.

The second assigned reading, "The Illusion of Algorithmic Fairness," demonstrates that attempts to reduce elements of fairness to mathematical equations have persisted throughout history. Discussions about algorithmic fairness today mirror many of the same points of contention reached in past debates about fairness, such as whether we should optimize for utility or optimize for fair outcomes. Consequently, fairness debates today have inherited some assumptions from these past discussions. In particular, we "take many concepts for granted including probability, risk, classification, correlation, regression, optimization, and utility." The author argues that despite our technical advances, fairness remains "irreducible to a mathematical property of algorithms, independent from specific social contexts." He shows that any attempt at formalism will ultimately be influenced by the social and political climate of the time. Moreover, researchers frequently use misrepresentative, historical data to create "fair" algorithms. The way that the data is framed and interpreted can be misrepresentative and frequently reinforces existing discrimination (for example, predictive policing algorithms predict future policing, not future crime.)

These readings set the stage for a conversation about how we should approach developing interventions. While "Discrimination in the Age of Algorithms" makes a strong case for using algorithms (in conjunction with counterfactuals) to improve the status quo and make it easier to prove discrimination in court, "The Illusion of Algorithmic Fairness" cautions against trying to reduce components of fairness to mathematical properties. The "Illusion of Algorithmic Fairness" paper shows that this is not a new endeavor. Humans have tried to standardize the concept of fairness as early as 1700 and we have proved time and again that determining what is fair and what is unfair is much too complicated and context dependent to model in an algorithm.

**Class Session 9: Intervening on behalf of interpretability**

In our second to last class, we discussed causal inference, how it differs from correlative machine learning techniques, and its benefits and drawbacks. We then considered how causal models could be deployed in the criminal justice context to generate individualized sentences and what an algorithmically informed individualized sentence would look like.

- The Book of Why by Judea Pearl and Dana Mackenzie, Basic Books (2018). Read Introduction.
- [State of Wisconsin v. Eric Loomis](http://www.scotusblog.com/wp-content/uploads/2017/02/16-6387-op-bel-wis.pdf) (2016), paragraphs 11-28 and 67-74.

The Book of Why describes the emerging field of causal inference, which attempts to model how the human brain works by considering cause and effect relationships. The introduction delves a little into the history of causal inference and explains that it took time for the field to develop because it was nearly impossible for scientists to communicate causal relationships using mathematical terms. We've now devised ways to model what the authors call "the do-operator" (which indicates that there was some action/form of intervention that makes the relationship causal rather than correlative) through diagrams, mathematical formulas and lists of assumptions.

One main point of the introduction and the book is that "data are dumb" because they don't explain why something happened. A key component of causal inference is the creation of counterfactuals to help us understand what would have happened had certain circumstances been different. The hope with causal inference is that it will be less impacted by bias because causal inference models do not look for correlations in data, but rather focus on the "do-operator." A causal inference approach may also make algorithms more interpretable because counterfactuals will offer a better way to understand how the AI makes decisions.

The other assigned reading, State of Wisconsin v. Eric Loomis, is a 2016 case about the use of risk assessment tools in the criminal justice system. In Loomis, the court used a risk assessment tool, COMPAS, to determine the defendant's risk of pretrial recidivism, general recidivism, and violent recidivism. The key question in this case was whether the judge should be able to consider the risk scores when determining a defendant's sentence. The State Supreme Court in this case decided that judges could consider the risk score because they also take into account other evidence when making sentencing decisions. For the purposes of this class, the case provided a lede into a discussion about the right to an individualized sentence and whether risk assessment scores can result in more fair outcomes for defendants. However, it turns out that risk assessment tools should not be employed if the goal is to produce individualized sentences. Despite their appearance of generating unique risk scores for defendants, risk assessment scores are not individualized as they compare information about an individual defendant to data about similar groups of offenders to determine that individual's recidivism risk.

**Class Session 10: Intervening against adversarial examples and course conclusion**

We opened our final class with a discussion about adversarial examples and technical debt before wrapping up the course with a final reflection on the broader themes and findings of the course.

- "[Hidden Technical Debt in Machine Learning Systems](https://perma.cc/PP9V-N4E6)" by D. Sculley et al., NIPS (2015)

The term "technical debt" refers to the challenge of keeping machine learning systems up to date. While technical debt is a factor in any type of technical system, machine learning systems are particularly susceptible to collecting a lot of technical debt because they tend to involve many layers of infrastructure (code and non code). Technical debt also tends to accrue more in systems that are developed and deployed quickly. In a time crunch, it is more likely that new features will be added without deleting old ones and that the systems will not be checked for redundant features or unintended feedback loops before they are deployed. In order to combat technical debt, the authors suggest several approaches including, fostering a team culture that encourages simplifying systems and eliminating unnecessary features and creating an alert system that signals when a system has run up against pre-programmed limits and requires review.

During the course retrospective, students identified several overarching themes of the class including, the effectiveness and importance of interdisciplinary learning, the tendency of policymakers and industry leaders to emphasize short term outcomes over long term consequences of decisions, the challenge of teaching engineers to consider the ethical implications of their work during the development process, and the lack of input from diverse groups in system design and deployment.

###### Credits

Syllabus Notes by Samantha L. Bates

Syllabus by Samantha Bates, John Bowers and Natalie Saltiel