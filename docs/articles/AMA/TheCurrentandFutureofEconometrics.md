The Current and Future of Econometrics
======================================

The AMA Interview with Prof. Jeffrey Wooldridge

**About Prof. Jeffrey Wooldridge**
==================================

![](https://miro.medium.com/max/1400/1*2mpvSzSjOAK75jRou7WNcA.png)<br />Figure  1: Prof. Jeffrey Wooldridge

Prof. Jeffrey Wooldridge is a University Distinguished Professor of Economics at Michigan State University, where he has taught since 1991. He is the author of two very popular econometrics textbooks, [Introductory Econometrics: A Modern Approach](https://www.cengage.com/c/introductory-econometrics-a-modern-approach-7e-wooldridge/9781337558860PF/), and [Econometric Analysis of Cross Section and Panel Data](https://mitpress.mit.edu/books/econometric-analysis-cross-section-and-panel-data-second-edition), one for undergraduates and one for graduates. Students at Duke and all over the world all study introductory econometrics using Prof. Wooldridge’s book.

![](https://miro.medium.com/max/790/1*j4xXUo4gKvGKc4RJebgJaw.jpeg)<br />Figure  2: Introductory Econometrics: A Modern Approach by Prof. Jeffrey Wooldridge

Known for his theoretical contributions to the analysis of cross-sectional and panel data, Prof. Wooldridge has published over 70 articles in internationally recognized journals, as well as several chapters in well-respected books. His work has earned many awards, including the Alfred P. Sloan Research Fellowship, the Plura Scripsit Award from Econometric Theory, the Sir Richard Stone prize from the Journal of Applied Econometrics, and three graduate teacher-of-the-year awards from MIT. A fellow of the Econometric Society, the Journal of Econometrics, and the International Association for Applied Econometrics, Dr. Wooldridge has been editor of the Journal of Business and Economic Statistics and econometrics co-editor of Economics Letters. Dr. Wooldridge received his Ph.D. in economics from the University of California, San Diego.

AMA Interview Video
===================

Watch our AMA Interview Video with Prof. Jeffrey Wooldridge on [YouTube](https://www.youtube.com/watch?v=j-ROW9jhcw4).

Interview Video

**Question 1**
==============

**William:**

> With so many years of experience in studying and teaching econometrics, what do you think are some most important principles people should keep in mind when learning and using econometrics? What are some most commonly made mistakes?

**Prof. Wooldridge:**

> That could be a very broad question, but I like the way you asked it in terms of basic concepts. I do think there is a tendency for students to jump ahead quickly to study measure theory, topology, other kinds of fancy math, thinking that those concepts are at the heart of modern econometrics. Don’t get me wrong: those can be quite useful for theoretical econometrics research, but for understanding how the basic econometric methods work, it’s really important to get a firm grounding in **basic probability**. Of course, after basic probability follows statistics. Much of our knowledge about regression analysis, for example, can be learned without looking at data first — understanding how one manipulates random variables and random vectors, understanding the notion of a linear projection and conditional expectations and how those get manipulated. That will actually take you pretty far for both linear analysis and the analysis of nonlinear models.
> 
> Then, one does need to learn concepts like **the standard limit theorems**, such as the Law of Large Numbers and the Central Limit Theorem (CLT) \[1\], and along with those limit theorems come many ways to manipulate sequences of random variables and random vectors. Becoming very good at that, so that those manipulations become second nature, allows one to focus on the interesting aspects of econometrics such as coming up with a new estimator or applying an estimator to an interesting set of data and then actually understanding when the estimator will work and when it won’t. That doesn’t require such high-level math, but it does require constantly going back and making sure that you know you haven’t missed anything and paying attention when you first study this material. Because we’re sometimes eager to jump into data analysis without having the formal background to understand completely even a simple method that we take for granted, like ordinary least squares. I am still getting new insights into that method, even just working on some recent research, in fact.

Question 2
==========

**Prof. Luyao Zhang:**

> We know econometrics has many intersections with statistics or machine learning theory. What do you think is the fundamental difference between the methodology of econometrics and other similar sciences? How do you define the boundary econometrics?

**Prof. Wooldridge:**

> This could be a controversial question because some people think that econometrics is just a subfield of statistics. I’ve heard people even question why econometrics is a field. However, we are supposed to, and most of us do, have training in economics. Therefore, we are supposed to focus on topics that at least arise in some economic setting.
> 
> Now I do think that because econometrics is studied by people who have Ph.D.s from economics departments, it is very similar to economics, and it really doesn’t see any boundaries. If you think of economics as a discipline, perhaps it’s a bit arrogant. However, we do tend to think that we can bring something to the analysis of almost every problem that involves people, firms, government agencies, and anything that involves interactions among units where there are incentives and outcomes.
> 
> Therefore, this attitude has spilled over into econometrics as well, where we don’t really think there are many boundaries in data analysis. A good example is the merging of machine learning with causal inference in econometrics over the past ten years. Machine learning methods started in statistics, which were largely used for prediction purposes. Econometricians have <br />Figure d out how to modify those methods and use them for causal inference. I don’t think there is any sense that some commission thinks this is out of boundary for us. The econometricians just say, “look, we’re interested in estimating the effects of policy interventions in causal analysis generally, and this is how these tools can be applied.”
> 
> I don’t really see the boundary in terms of applied econometrics. All you have to do is to pick up one of either top five general purpose journals or look at the top field journals. Then, you will see topics ranging from criminology to health issues, where in some cases, you might think these would be things studied by epidemiologists or criminal justice people. Yet economists are involved in all of these. Look at what has happened with evaluating the effects of the coronavirus. Economists have been involved with that a lot and tried to <br />Figure  out what the economic costs are, even including what the psychological costs of the virus are, how effective things like lockdowns are, and so on. Therefore, I do not see many boundaries between economists and econometricians.

**Question 3**
==============

**William:**

> Your recent Econometrica paper ([Abadie et al. 2020](https://doi.org/10.3982/ECTA12675)) discusses an alternative way of interpreting standard errors in regressions as design-based uncertainty, in addition to the traditional sample-based uncertainty. Would you like to elaborate more on this paper? What does this result mean to the empirical researchers? When should we interpret standard errors in a design-based way, as suggested in the paper?

![](https://miro.medium.com/max/1400/1*VDAa8OzoJjrShr22NwC1SA.png)<br />Figure  3: [Sampling-Based versus Design-Based Uncertainty in Regression Analysis](https://doi.org/10.3982/ECTA12675)

**Prof. Wooldridge:**

> Thanks for this question. We’re still working together on the paper, and we extend the initial work to the case where one might have to cluster the standard errors to account for either cluster sampling or some clustering in the design itself, the assignment of the treatment and the control groups. Then, we realized that we didn’t actually fully understand the non-clustering case where we were taking random samples.
> 
> We would think about not necessarily randomly assigning a policy, but where the assignment was independent across the units. This question used to come up to me. Occasionally, students would say, “you’ve taught us how to analyze ordinary least squares \[2\], the asymptotic properties from the perspective of taking a random sample from the population, but what happens if you observe the entire population?”, which is a great question because we often do, especially with aggregated data at the county level (e.g. counties, provinces). You see all of them.
> 
> When you do any kind of econometric method like ordinary least squares (OLS), how do you interpret the standard errors that are reported? We decided to try to bridge this gap. There’s been a long history in the design-based approach. The statisticians were involved many years ago and thought about having the population data. There’s no sampling, but what you do have is that you have potential outcomes in both a control state and a treated state. Then, all the uncertainty comes through assigning units to the control or the treated.
> 
> Now, the randomness comes from the situation where we only observe each unit in one state of the world. The way we assign the treatment is random. My books focus a lot on the random sampling case, so it seemed natural to try to come up with a framework to bring those two together. The framework provides a smooth transition from the case where you have random sampling from a large population all the way to the case where there’s no sampling, and you observe the entire population. We manage to come up with a formula that covers all those cases. You can see explicitly that the formula for the proper variance depends on the fraction of the population that you observe.
> 
> Therefore, one of the important insights that comes out of this is that **if you observe the whole population and use the usual standard errors, they are conservative**, so your confidence intervals are wider than they need to be in general. There are some cases where they’re not conservative, when there is no underlying heterogeneity in the effects across people. There are cases where the usual heteroscedasticity-robust standard error, the so-called Eicker–Huber–White standard errors, are the right ones. But in general, they are conservative. Therefore, at least for now, if you have the whole population, you’re using conservative errors.
> 
> We actually have something in the paper that hasn’t been applied as much, which is when you do observe the whole population or a significant fraction of the population, there’s a way to adjust your standard errors to make them smaller. It’s making them smaller in a legitimate way, because as you observe more of the population, the sampling error becomes less. Our paper shows exactly how the adjustment works, which is quite simple. Once somebody programs this up in Stata, I hope that it’ll be used quite regularly. Moreover, there’s some simple tricks to use it now based on using formulas from the stratified sampling literature, which also has a history in statistics. All of this research draws on lots of different fields, and it’s becoming very interdisciplinary.

Question 4
==========

**Prof. Luyao Zhang:**

> In the past years, you have done much work improving our knowledge on some widely used econometric models, including instrument variables, difference-in-difference, and treatment effects ([Słoczyński and Wooldridge 2018](https://doi.org/10.1017/S0266466617000056); [Wooldridge 2019](https://doi.org/10.1016/j.jeconom.2018.12.010); [Wooldridge 2021](http://dx.doi.org/10.2139/ssrn.3906345)). How do you think these new findings will influence the way empirical researchers apply these models? In which scenarios should we apply these new models? More generally, how do you think empirical researchers should learn about the latest econometric methods?

![](https://miro.medium.com/max/1008/1*zenxD26MQWAKQ5qj15kE4A.png)<br />Figure  4: Intuition of difference-in-difference

**Prof. Wooldridge:**

> Of course, I hope empirical people would use my research regularly. You’ve mentioned a few topics that I’ve been working on, and I do continue to work on those.
> 
> One of the methods that has become quite useful recently by combining methods from traditional treatment effects \[3\] with difference-in-difference \[4\] is the so-called doubly robust estimators that again have a history of statistics. I worked on this more than 15 years ago. I published a paper in 2007 in the Journal of Econometrics ([Wooldridge 2007](https://doi.org/10.1016/j.jeconom.2007.02.002)) that proposed a particular kind of doubly robust estimator. If you’re estimating a treatment effect, typically there are two approaches. Maybe more than two, but I will focus on two. You can use regression adjustment, which means you estimate models for the conditional mean of the outcome variable; You can use some propensity score method, which means you estimate a model for the treatment. It has been known for a while that you can combine those two to come up with an estimator which has a doubly robust property. The name is maybe not quite the right one, but it means that you only have to have one of the two models correct in order to consistently estimate the average treatment effect. That was derived in the context of cross-sectional analysis, but it turns out to be noticed by other researchers. And then something I’m working on is that you can apply these robust methods to the panel data case as well, when you have difference-in-difference-type designs in a policy intervention. You have data before and after; you have a control group and a treatment group, and it turns out that you can apply this to even fairly complicated structures with staggered designs.
> 
> You did mention the difference-in-difference work, so let me focus on what I’ve actually written about. I think this is generally a good lesson that I showed **you can use traditional regression methods**. In particular, you can expand the usual two-way fixed effects estimator. Actually, it’s not expanding the estimator, but expanding the model. My interpretation of the recent criticism of two-way fixed effects is that it’s not a criticism of the estimator but a criticism of the model. The model assumes a single treatment effect, regardless of how many cohorts there are and how long the time period is for the intervention. And I simply noted that if you set things up properly, you can apply regression methods to estimate a much more flexible model, and this largely overcomes the criticisms of the simple two way fixed effects analysis.
> 
> So, what I tried to emphasize with my students is that **it’s very important to keep separate the notion of a model and an estimation method**. And I sometimes forget myself. I will say things like OLS model, but OLS is not a model. It’s an estimation method which we can apply to various kinds of models. It’s up to us to be creative and use the tools that we have so that we apply those methods to models that don’t make strong assumptions. I hope that this idea bridges again a lot of my research, which is pretty simple. It’s trying to find simpler ways to do more flexible analysis, at the point that it gets really hard.

Question 5
==========

**William:**

> On your Twitter, you criticized that machine learning is “running simulations until my new estimator looks notably better than existing estimators”. Can you elaborate on your thoughts on how machine learning and other high-dimensional methods can improve in order to contribute to the field of economics and econometrics?

![](https://miro.medium.com/max/1400/1*hquzlKwJx-V1e-VrWFv2AA.png)<br />Figure  5: Machine Learning

**Prof. Wooldridge:**

> Posting on Twitter is a bit different than actually writing a serious research paper. But I was, of course, partly making a joke there because I was in the middle of doing some simulations for some recent nonlinear difference-in-differences methods that I’ve been working on. But then I was thinking, as I was doing the simulations and changing the parameters of the simulations, am I doing this to learn about how this estimator compares with other estimators, or am I trying to rig it so that my estimator looks the best? So, I was really just making a statement. Like you know, it’s human nature to want yours to be the best, right? One uses the machine to learn about that, and I’m partly making a statement. I’m trying to be as objective as I can by showing cases where the methods I’m proposing work better but also being upfront about cases where other methods will work better.
> 
> It’s not completely unrelated to machine learning, though. When we publish papers, the best way to get your work published is to show that it works better than existing methods. Since the people writing the theory and deriving the methods are the same ones doing the simulations, it will probably be better if there’s some disconnection there. We have some ways of objectively evaluating these methods now. If something becomes popular enough, others will evaluate it. But I think simulations are still needed to know about how something works in the real world.
> 
> I’ve always thought that we should have more competitions, such as blind competitions where people who participate don’t know what the truth is. They apply their favorite method across a bunch of different scenarios, so we can evaluate how the different methods do. I’m guessing that machine learning will come out pretty well with that, but that’s an impression. I’m not convinced that somebody using basic methods who has good intuition and is creative can’t do as well.
> 
> This does raise the issue of machine learning and its future. I’m sure you’ve seen in your data analysis, where this has to have come up a fair amount. I think the work on applying machine learning methods to causal inference has guaranteed that it will have a long history in econometrics and other fields that use data analysis. When I took visits to campuses, Amazon, Google, they’re using machine learning methods quite a bit. That’s no secret. These companies are in the business of earning profits, and they’re not going to employ methods that somehow aren’t working for them. So, I think the market is certainly speaking on that. For prediction purposes, they seem to work very well.

Reflections
===========

**Prof. Luyao Zhang:**

> Yes, sounds very interesting! Prof. Wooldridge points out promising directions for machine learning from just a prediction to find more scientific results. You can have machine learning plus causal inference. Zichao and Yufan are both from the data science major, so it will be great to hear their comments, especially those about the econometrics and machine learning.

**Yufan Zhang:**

> Prof. Wooldridge’s point about machine learning resonates with me as a data science student. The more I study some advanced machine learning models, especially deep learning models, the more I feel that it’s unscientific. Many newly proposed models today are very functional and well-performed but also very complicated. Most of what the researchers are doing is just to try different models, such as adding different modules to the model. If the result of one structure doesn’t work, they just try another one. So I think that’s indeed the problem that the whole machine learning is, especially deep learning, is facing now.

**Prof. Jeffrey Wooldridge:**

> It is a very good observation. Since I’ve only dabbled in machine learning a bit, I don’t have the experience that you have on how people are using it and progressing. Probably at the end, it’s just like other econometric methods where people try a lot of different things, and they only report the one that gives the result that they want. So, perhaps machine learning hasn’t saved us from that as much as we’re being led to believe it. There is a bait. Just to follow up on that, I’ve seen plenty of papers that jump right into the very difficult thing, which misses the low hanging fruit. In other words, there are simple ways to do things like causal inference. For example, one can estimate causal effects with instrumental variables to exploit the structure in ways that haven’t been exploited before, instead of going fully to machine learning, the black box. It would be good if people try things that are easier to understand and then see if the more difficult thing produces similar answers or not.

**Zichao Chen:**

> The world is changing rapidly. With the emergence of blockchain and many other information technologies, the problems in economics are becoming more complicated. What do you think is the trend of development in econometrics?

**Prof. Wooldridge:**

> That’s a really interesting and actually tough question for me. It’s interesting that if you look at the literature on intervention analysis and difference-in-difference, in some ways we’re trying to go back to simpler things. So, if you were to compare today with twenty years ago and see what econometrics people are doing, it seems to me that structural methods may be more out of favor now than they were fifteen years ago with this re-emergence of difference-in-difference. It seems that we are always looking for natural experiments and interventions to learn things about policy.
> 
> If you have a lecture, and you have difference-in-difference in the title, or you offer a short course, immediately you will get a fairly large enrollment. But if you were offering a course on structural econometric methods in industrial organization, which is important, it seems to have a smaller audience. So, I wonder if our reaction to these complications in the real world is leading us to simplify the econometrics. Or, at least we are going to only believe analyses that have some clear way to identify the causal effect of an intervention rather than our relatively simple economic models.

Relevant Materials
==================

1.  [**Central Limit Theorem (CLT)**](https://en.wikipedia.org/wiki/Central_limit_theorem): In probability theory, the central limit theorem (CLT) establishes that, in many conditions, when independent random variables are summed up, their properly normalized sum tends toward a normal distribution (informally a bell curve) even if the original variables themselves are not normally distributed.
2.  [**Ordinary Least Squares (OLS)**](https://en.wikipedia.org/wiki/Ordinary_least_squares): an estimation method of regression models that aim to minimize the sum of the squares of the differences between the observed dependent variable (values of the variable being observed) in the given dataset and those predicted by the linear function of the independent variable.
3.  [**Treatment Effect**](https://en.wikipedia.org/wiki/Average_treatment_effect): the difference in potential outcomes between an unit assigned to the treatment and the unit assigned to the control. Usually only one of the two potential outcomes is observed in data, because a unit can either be assigned to the treatment or the control.
4.  [**Difference-in-differences**](https://en.wikipedia.org/wiki/Difference_in_differences) **(DID)**: an econometric model that estimate the effect of a treatment (i.e., an explanatory variable or an independent variable) on an outcome (i.e., a dependnet variable) by comparing the average change over time in the outcome variable for the treatment group to the average change over time for the control group.

Acknowledgments
===============

Interviewee: Prof. Jeffrey Wooldridge

Interviewer: Prof. Luyao Zhang, William Zhao

Discussants: Zichao Chen, Yufan Zhang

Executive Editors: Xinyu Tian, Ray Zhu

Chief Editor: Prof. Luyao Zhang
