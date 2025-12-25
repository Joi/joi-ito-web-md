---
title: "2019 Applied Ethical and Governance Challenges in AI - Notes from Part 2: Prognosis"
date: 2019-03-26T00:00:00
permalink: https://joi.ito.com/weblog/2019/03/26/applied-ethical.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2019/03/26/applied-ethical.html
extracted: 2025-12-25
---

This is the second of three parts of the syllabus and summaries prepared by Samantha Bates who TAs the Applied Ethical and Governance Challenges in Artificial Intelligence course which I co-teach with Jonathan Zittrain. John Bowers and Natalie Satiel are also TAs for the course. [I posted Part I](https://joi.ito.com/weblog/2019/03/07/2019-applied-et.html) earlier in the month.

My takeaways:

In Part I, we defined the space and tried to frame and understand some of the problems. We left with concerns about the reductionist, poorly defined and oversimplified notions of fairness and explainability in much of the literature. We also left feeling quite challenged by how the technical community will face new risks such as adversarial attacks and approaches like it.

In Part II, we continue our journey into a sense of despair about AI ethics and governance. In Solon Barocas and Andrew D. Selbst's paper "Big Data's Disparate Impact," they walk us through the state of the law around discrimination and fairness using Title VII of the US Civil Rights Act as an example. The authors show us that while it was enacted to address discrimination concerns raised by the civil rights movement, the law has evolved away from trying to correct societal inequities through remedies such as affirmative action. Instead, the law has focused more and more on fairness of processes and less on redistribution or on resolving historical inequity. As a result, the law has adopted a more technical notion of fairness - a kind of actuarial "all lives matter" sort of approach. During Part I, when we discussed the biased [Amazon hiring tool](https://www.reuters.com/article/us-amazon-com-jobs-automation-insight/amazon-scraps-secret-ai-recruiting-tool-that-showed-bias-against-women-idUSKCN1MK08G), one of the proposed remedies was to "put our thumb on the scale" and just boost the scores of women and minorities. The Barocas and Selbst paper demonstrates that this type of solution is no longer supported by the law. The sense is that the engineers thought, "of course there must be a law prohibiting discrimination, we can use that." In fact, that law punts on redistribution or societal inequity. Jonathan pointed out that treatment of social inequality in Tort law is similar. If you run over a rich person and a poor person at the same time, you have to pay the rich family more - the calculation of damages is based on the victim's future earning power. Tort law, like Title VII, says, "there may be societal inequities, but we're not solving that problem here."

Sandra Wachter's paper proposing counterfactuals as a way to provide explainability is an excellent idea and feels like one way forward in the explainability debate. However, even Sandra seems concerned about whether laws such as the GDPR will actually be able to require companies to provide such explanations. We also had some concerns about the limits of counterfactuals in identifying biases or providing the "best" answer depending on the person - limits Sandra identifies in her paper.

Finally, we take adversarial attacks from the theoretical to a specific example in [a recent paper](http://science.sciencemag.org/content/363/6433/1287) that Jonathan and I wrote with John Bowers, Samuel Finlayson, Andrew L. Beam, and Isaac S. Kohane about the risks of adversarial attacks on medical AI systems.

Please see Samantha's summaries and links to the readings below for a more complete overview of the three classes in Part II.

- Joi

**Part 2: Prognosis**

*By Samantha Bates*

**Syllabus Notes: Prognosis Stage**

Welcome to part 2 of our Ethical and Governance Challenges in AI syllabus! In part 1, the assigned readings and class discussion focused on understanding how the social, technical, and philosophical roots of autonomous systems contribute to problems related to fairness, interpretability, and adversarial examples. In the second stage of the course, the prognosis stage, the class considered the social implications of these problems. Perhaps the most significant takeaway from this stage was the realization that many of these problems are social or political problems and cannot be addressed through solely a legal or technical approach.

**Class Session 5: Prognosticating the impacts of unfair AI**

Solon Barocas, an Assistant Professor at Cornell University, joined the class for the first day of the prognosis stage. We discussed his paper, "Big Data's Disparate Impact," which offered a legal and technical perspective on the use of algorithms in employment.

- "[Big Data's Disparate Impact](https://perma.cc/YFW7-36L7)" by Solon Barocas and Andrew D. Selbst, California Law Review (2016)

On the first day of the prognosis stage, the focus of the class shifted from examining the technical mechanisms underlying autonomous systems to looking at the societal impact of those systems. The Barocas and Selbst paper discusses how data collection and data labeling can perpetuate existing biases both intentionally and unintentionally. The authors outline five main ways that datasets can be discriminatory:

1. Our own human biases may be integrated into a dataset when a human data miner determines the parameters that an autonomous system will use to make decisions.
2. The training data might already be biased depending on how it was collected and how it was labeled.
3. Data mining models consider a limited number of data points and thus may draw conclusions about an individual or a group of people based on data that is not representative of the subject.
4. As Cathy O'Neil mentioned, prejudice may be introduced if the data points the model uses to make decisions are proxies for class membership.
5. Discriminatory data mining could be intentional. However, the authors argue that unintentional discrimination is more common and harder to identify.

While there is legal doctrine that addresses discrimination in employment, the authors demonstrate that it is difficult to apply in practice, particularly in the data mining context. Title VII creates liability for intentional discrimination (disparate treatment) and for unintentional discrimination (disparate impact), but it is difficult to prove either type. For example, in order to hold employers liable for unintentional discrimination, the plaintiff must show that an alternative, nondiscriminatory method exists that will accomplish the same goals as the discriminatory practice. They must also prove that when presented with the alternative, the employer refused to consider it. Typically, an employer can mount a successful defense if they can prove they were unaware of the alternative or if there is a legitimate business reason for policies that may be discriminatory (the business necessity defense).

Bias in data mining is so difficult to identify, prove, and rectify in part because as a society, we have not determined the role of the law in addressing discrimination. According to one theory, the anticlassification theory, the law has an obligation to ensure that decision makers do not discriminate against protected classes in society. The opposing theory, the antisubordination theory, advocates a more hands-on approach and states that the law should work to "eliminate status-based inequality" at the societal level by actively improving the lives of marginalized groups. Our current society favors the anticlassification approach in part because the court established early on that antidiscrimination law was not solely intended to improve access to opportunities for protected classes. And while the authors demonstrate how data mining can exacerbate existing biases in the hiring context, there is a societal trade-off between prioritizing efficient decision making and eliminating bias.

This reading also raises the question of who is responsible for fixing the problem. Barocas and Selbst emphasize that the majority of data mining bias is unintentional and that it may be very difficult to identify bias and employ technical fixes to eliminate it. At the same time, there are political and social factors that make fixing this problem in the legal system equally difficult, so who should be in charge of addressing it? The authors suggest that as a society, we may need to reconsider how we approach discrimination issues more generally.

**Class Session 6: Prognosticating the impacts of uninterpretable AI**

For our sixth session, the class talked with Sandra Wachter, a lawyer and research fellow at the Oxford Internet Institute, about the possibility of using counterfactuals to make autonomous systems interpretable.

- "[Counterfactual Explanations Without Opening the Black Box: Automated Decisions and the GDPR](https://perma.cc/TPX7-Y689)" by Sandra Wachter et al., Harvard Journal of Law and Technology (2018)
- [OPTIONAL] "[Algorithmic Transparency for the Smart City](https://perma.cc/EFQ3-MH9F)" by Robert Brauneis & Ellen P. Goodman, Yale Journal of Law and Technology (2018)

In our last discussion about interpretability, the class concluded that it is impossible to define the term "interpretability" because it greatly depends on the context of the decision and the motivations for making the model interpretable. The Sandra Wachter et al. paper essentially says that defining "interpretability" is not important and that instead we should focus on providing a way for individuals to learn how to change or challenge a model's output. While the authors point out that making these automated systems more transparent and devising some way to hold them accountable will improve the public's trust in AI, they primarily consider how to design autonomous models that will meet the explanation requirements of the GDPR. The paper's proposed solution is to generate counterfactuals for individual decisions (both positive and negative) that "provide reasons why a particular decision was received, offer grounds to contest it, and provide limited 'advice' on how to receive desired results in the future."

Not only would counterfactuals exceed the explainability requirements of the GDPR, the authors argue that counterfactuals would lay the groundwork for a legally binding right to explanation. Due to the difficulty of explaining the technical workings of an automated model to a lay person, legal concerns about protecting trade secrets and IP, and the danger of violating the privacy of data subjects, it has been challenging to provide more transparency around AI decision making. However, counterfactuals can serve as a workaround to these concerns because they indicate how a decision would change if certain inputs had been different rather than disclose information about the internal workings of the model. For example, a counterfactual for a bank loan algorithm might tell someone who was denied a loan that if their annual income had been $45,000 instead of $30,000, they would have received the loan. Without explaining any of the technical workings of the model, the counterfactual in this example can tell the individual the rationale behind the decision and how they can change the outcome in the future. Note that counterfactuals are not a sufficient solution to problems involving bias and unfairness. It may be possible for counterfactuals to provide evidence that a model is biased. However, because counterfactuals only show dependencies between a specific decision and particular external facts, they cannot be relied upon to expose all potential sources of bias or confirm that a model is not biased.

The optional reading, "Algorithmic Transparency for the Smart City," investigates the transparency around the use of big data analytics and predictive algorithms by city governments. The authors conclude that poor documentation and disclosure practices as well as trade secrecy concerns frequently prevented city governments from getting the information they needed to understand how the model worked and its implications for the city. The paper expands upon the barriers to understanding an autonomous model that are mentioned in the Watcher et. al. paper and also presents a great example of scenarios in which counterfactual explanations could be deployed.

**Class Session 7: Prognosticating the impacts of adversarial examples**

In our third prognosis session, the class continued its discussion about adversarial examples and considered potential scenarios, specifically in medical insurance fraud, in which they could be used to our benefit and detriment.

- "Adversarial attacks on artificial intelligence systems as a new healthcare policy consideration" by Samuel Finlayson, Joi Ito, Jonathan Zittrain et al., preprint (2019)
- "[Law and Adversarial Machine Learning](https://perma.cc/W46R-2GL7)" by Ram Shankar Siva Kumar et al., ArXiv (2018)

In our previous session about adversarial examples, the class discussion was primarily focused on understanding how adversarial examples are created. The readings delve more into how adversarial examples can be used to our benefit and also to our detriment. "Adversarial attacks on artificial intelligence systems as a new healthcare policy consideration" considers the use of adversarial examples in health insurance fraud. The authors explain that doctors sometimes use a practice called "upcoding", when they submit insurance claims for procedures that are much more serious than were actually performed, in order to receive greater compensation. Adversarial examples could exacerbate this problem. For instance, a doctor could make slight perturbations to an image of a benign mole that causes an insurance company's autonomous billing code infrastructure to misclassify it as a malignant mole. Even as insurance companies start to require additional evidence that insurance claims are valid, adversarial examples could be used to trick their systems.

While insurance fraud is a serious problem in medicine, it is not always clearly fraudulent. There are also cases when doctors might use upcoding to improve a patient's experience by making sure they have access to certain drugs or treatments that would ordinarily be denied by insurance companies. Similarly, the "Law and Adversarial Machine Learning" paper encourages machine learning researchers to consider how the autonomous systems they build can both benefit individual users and also be used against them. The authors caution researchers that oppressive governments may use the tools they build to violate the privacy and free speech of their people. At the same time, people living in oppressive states could employ adversarial examples to evade the state's facial recognition systems. Both of these examples demonstrate that deciding what to do about adversarial examples is not straightforward.

The papers also make recommendations for crafting interventions for problems caused by adversarial examples. In the medical context, the authors suggest that the "procrastination principle," a concept from the early days of the internet that argued against changing the Internet's architecture to preempt problems, might be applicable to adversarial examples as well. The authors caution that addressing problems related to adversarial examples in healthcare too early could create ineffective regulation and prevent innovation in the field. Instead the authors propose extending existing regulations and taking small steps, such as creating "fingerprint" hashes of the data submitted as part of an insurance claim, to address concerns about adversarial examples.

In the "Law and Adversarial Machine Learning" paper, the authors emphasize that lawyers and policymakers need help from machine learning researchers to create the best machine learning policies possible. As such, they recommend that machine learning developers assess the risk of adversarial attacks and evaluate existing defense systems on their effectiveness in order to help policymakers understand how laws may be interpreted and how they should be enforced. The authors also suggest that machine learning developers build systems that make it easier to determine whether an attack has occurred, how it occurred and who might be responsible. For example, designers could devise a system that can "alert when the system is under adversarial attack, recommend appropriate logging, construct playbooks for incident response during an attack, and formulate a remediation plan to recover from an attack." Lastly, the authors remind machine learning developers to keep in mind how machine learning and adversarial examples may be used to both violate and protect civil liberties.

###### Credits

Notes by Samantha Bates

Syllabus by Samantha Bates, John Bowers and Natalie Saltiel