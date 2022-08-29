---
layout: post
---
#### Organizers 
Anastasios Tsiamis (ETH), Ingvar Ziemann (KTH), Nikolai Matni (UPenn) George Pappas (UPenn)\
**Contact:** [atsiamis@control.ee.ethz.ch](atsiamis@control.ee.ethz.ch), [ziemann@kth.se](ziemann@kth.se)

#### Relevant Links
- [IEEE CDC 2022 Workshops](https://cdc2022.ieeecss.org/workshop/)
- [IEEE CDC 2022 Registration](https://cdc2022.ieeecss.org/registration/)

## Motivation and Objectives

<div align="justify">Machine learning methods are at an ever increasing pace being integrated into domains that have classically been within the purview of controls. There is a wide range of examples, including perception-based control, agile robotics, and autonomous driving and racing. As exciting as these developments may be, they have been most pronounced on the experimental and empirical sides. To deploy these systems safely, stably, and robustly into the real world, we argue that a principled and integrated theoretical understanding of a) fundamental limitations and b) statistical optimality is needed. With this workshop we seek to bring together theoretical research across machine learning and control theory to address these issues in tasks like system identification, learning-based control and estimation. This workshop will serve as a good reference for a wider audience as to what the current state of the art in this intersection is. We also aim to make existing technical tools in this area more accessible to an audience with a control theoretic background, as they require mathematical tools not typically included in a control theorist’s training (e.g., high-dimensional statistics and learning theory). It is our hope that this workshop also serves as a good reference for a younger audience as to what the current state of the art in this intersection is. 

The objective is to grow and foster the new interdisciplinary community around machine learning and control, with an emphasis on how mathematical methods from learning theory interact with classical control theoretic notions. To do so, we have invited speakers from both control and machine learning backgrounds. Talks will emphasize the interplay between control-theoretic notions, such as controllability, safety, stability, robustness, and learning theoretic notions, such as sample complexity, regret, and excess risk. We will revisit recent results for linear systems but also present recent advances in the case of more general nonlinear systems.

## Program
Times and dates will be updated soon. 

#### Confirmed talks
<details>
  <summary> 
    <i>Sample complexity analysis of input/output model identification: representations, over-parameterization, and self-regularization</i>, <strong>Necmiye Ozay (UMich Ann Arbor)</strong> </summary>
  <br>
  
  **Abstract:** In this talk we will review recent results on learning linear dynamical systems from input/output data. There are many different representations for linear systems like state space models, autoregressive models, impulse response. We show, in all these different settings, the learning accuracy for the ordinary least squares (OLS) estimator scales with one over the square root of the sample size, matching the sample complexity results in the static linear estimation problems. We will also highlight how some of the classical asymptotic system identification results can be recovered as special cases of our analysis framework. As an example, we will illustrate why overparameterization in an autoregressive model with external inputs does not lead to overfitting thanks to OLS having a self-regularization type property, which allows automatic recovery of system orders.
  
  **Biography:** Necmiye Ozay received her B.S. degree from Bogazici University, Istanbul in 2004, her M.S. degree from the Pennsylvania State University, University Park in 2006 and her Ph.D. degree from Northeastern University, Boston in 2010, all in electrical engineering. She was a postdoctoral scholar at the California Institute of Technology, Pasadena between 2010 and 2013. She joined the University of Michigan, Ann Arbor in 2013, where she is currently an associate professor of Electrical Engineering and Computer Science. She is also a member of the Michigan Robotics Institute. Dr. Ozay’s research interests include hybrid dynamical systems, control, optimization and formal methods with applications in cyber-physical systems, system identification, verification \& validation, autonomy and dynamic data analysis. Her papers received several awards. She received the 1938E Award and a Henry Russel Award from the University of Michigan for her contributions to teaching and research, and five young investigator awards, including NSF CAREER. She is also a recipient of the 2021 Antonio Ruberti Young Researcher Prize from the IEEE Control Systems Society for her fundamental contributions to the control and identification of hybrid and cyber-physical systems.
</details>

<details>
  <summary> 
    <i>Linear Systems Can Be Hard to Learn</i>, <strong>Anastasios Tsiamis (ETH Zurich)</strong> </summary>
  <br>
  
  **Abstract:** In this talk, we will discuss the statistical difficulty of learning-based control and system identification in linear systems. We focus on three topics, the sample complexity of system identification, the sample complexity of stabilization, and the regret of the online Linear Quadratic Regulator (LQR). Prior results state that the statistical difficulty for such benchmarks scales polynomially with the system state dimension up to system-theoretic quantities. However, this does not reveal the whole picture. By utilizing minimax lower bounds, we prove that there exist non-trivial classes of systems for which learning complexity scales dramatically, i.e. exponentially, with the system dimension.
This situation arises in the case of underactuated systems, i.e. systems with fewer inputs than states. Such systems are structurally difficult to control and their
system theoretic quantities can scale exponentially with the system dimension dominating learning complexity. In other words, systems with ill-conditioned controllability structure are hard to learn. Conversely, under some additional structural assumptions, i.e. bounding systems away from uncontrollability, learning complexity can be at most exponential with the controllability index of the system, that is the degree of underactuation. Hence, systems with robust controllability structure are easy to learn.
This is joint work with Ingvar Ziemann, Nikolai Matni, Manfred Morari, and George Pappas.
  
  **Biography:**  Anastasios Tsiamis is currently a postdoctoral researcher in the Automatic Control Laboratory, at ETH Zurich. He received his Ph.D. degree in electrical and systems engineering from the University of Pennsylvania (UPenn), Philadelphia, in 2022, under the supervision of George Pappas. He received his Diploma degree in electrical and computer engineering from the National Technical University of Athens, Greece, in 2014. His research interests include statistical learning for control, risk-aware control and optimization, and networked control systems. Anastasios Tsiamis was a finalist for the IFAC Young Author Prize in IFAC 2017 World Congress and a finalist for the Best Student Paper Award in ACC 2019.
</details>

<details>
  <summary> 
    <i>Learning from many trajectories</i>, <strong>Stephen Tu (Google Brain)</strong> </summary>
  <br>
  
  **Abstract:** We initiate a study of supervised learning from many independent sequences ("trajectories") of non-independent covariates, reflecting tasks in sequence modeling, control, and reinforcement learning.  Conceptually, our multi-trajectory setup sits between two traditional settings in statistical learning theory: learning from independent examples and learning from a single auto-correlated sequence.  Our conditions for efficient learning generalize the former setting--trajectories must be non-degenerate in ways that extend standard requirements for independent examples. They do not require that trajectories be ergodic, long, nor strictly stable.
For linear least-squares regression, given $n$-dimensional examples produced by m trajectories, each of length $T$, we observe a notable change in statistical efficiency as the number of trajectories increases from a few (namely $m \leq n$) to many (namely $m\geq n$).  Specifically, we establish that the worst-case error rate for this problem is $n/(mT)$ whenever $m \geq n$.  Meanwhile, when $m \leq n$, we establish a (sharp) lower bound of $n^2/(m^2 T)$ on the worst-case error rate, realized by a simple, marginally unstable linear dynamical system.  A key upshot is that, in domains where trajectories regularly reset, the error rate eventually behaves as if all of the examples were independent altogether, drawn from their marginals.  As a corollary of our analysis, we also improve guarantees for the linear system identification problem. 
This is joint work with Roy Frostig and Mahdi Soltanolkotabi. 
  
  **Biography:**  Stephen Tu is a research scientist in the Google Brain robotics team in NYC. He obtained his PhD in EECS from UC Berkeley under the supervision of Ben Recht. Broadly speaking, his research is focused on understanding the statistical complexity of learning to control. 
</details>


<details>
  <summary> 
    <i>Minimal Expected Regret in Linear Quadratic Systems</i>, <strong>Yassir Jedra (KTH)</strong> </summary>
  <br>
  
  **Abstract:**   We consider the problem of online learning in Linear 
Quadratic Control systems whose state transition and state-action 
transition matrices A and B may be initially unknown. We devise an 
online learning algorithm and provide guarantees on its expected 
regret. The regret  scalings we obtain are minimal in the time horizon 
and input and output dimensions  and match existing lower bounds. Existing online algorithms proceed  in epochs of 
(typically exponentially) growing durations.  The control policy is fixed 
within each epoch, which considerably simplifies the analysis of the 
estimation error on A and B and hence of the regret. Our algorithm  departs 
from this design choice: it is a simple variant of certainty-equivalence 
regulators, where the estimates of A and B and the resulting control 
policy can be updated as frequently as we wish, possibly at every step. 
Quantifying the impact of such a constantly-varying control policy on 
the performance of these estimates and on the regret constitutes one 
of the technical challenges tackled in this paper.
  
  **Biography:**  Yassir Jedra received a B.Sc. degree in 2015 and 
a M.Sc. degree in mathematics and computer science 
in 2018 from ENSIMAG Ecole National Superieure 
d’Informatique et de Mathematiques Appliquees, Grenoble, 
France; and a M.Sc. degree in Applied and Computational
Mathematics in 2018, from KTH The Royal Institute of 
Technology, Stockholm, Sweden. He is currently a Ph.D. 
student within the Division of Decision and Control Systems 
at KTH.
</details>



<details>
  <summary> 
    <i>Safe Adaptive Learning for Linear Quadratic Regulators with Constraints</i>,  <strong>Na Li (Harvard)</strong></summary>
  <br>
  
  **Abstract:**   We consider single-trajectory adaptive/online learning for linear quadratic regulator (LQR)  with an unknown system  and  constraints on  the states and actions.  The major challenges are two-fold: 1) how to ensure safety without  restarting the system, and 2) how to mitigate the inherent tension among exploration, exploitation, and safety.  To tackle these challenges, we propose a single-trajectory learning-based control algorithm that guarantees safety with high probability. Safety is achieved by robust certainty equivalence and a  SafeTransit algorithm. Further, we provide a sublinear regret bound compared with the optimal safe linear policy.  When developing the regret bound, we also establish a novel estimation error bound for nonlinear policies, which can be interesting on its own.
Joint work with: Yingying Li, Tianpeng Zhang, Subhro Das, Jeff Shamma, and Na Li
  
  **Biography:**  Na Li is a Gordon McKay professor in Electrical Engineering and Applied Mathematics at Harvard University.  She received her B.S. degree in Mathematics from Zhejiang University in 2007 and Ph.D. degree in Control and Dynamical systems from California Institute of Technology in 2013. She was a postdoctoral associate at the Massachusetts Institute of Technology 2013-2014.  Her research lies in the control, learning, and optimization of networked systems, including theory development, algorithm design, and applications to cyber-physical societal systems. She received the NSF career award, AFSOR Young Investigator Award, ONR Young Investigator Award,  Donald P. Eckman Award, McDonald Mentoring Award, along with some other awards.
</details>

<details>
  <summary> 
    <i>Smoothed Online Learning for Planning in Piecewise Affine Systems</i>, <strong>Max Simchowitz (MIT) </strong></summary>
  <br>
  
  **Abstract:** Piecewise affine systems are a powerful tool for modeling and planning through possibly nonlinear dynamics. In this talk, we develop a theory of the statistical complexity of iterative replanning in piecewise affine systems. In order to separate the challenges of exploration from those of system identification, we consider a new notion of “planning regret”, which measures the cumulative error between a learner’s forecasted dynamics and those of the best-possible piecewise affine system in hindsight, over a sequence of K replanning episodes. Intuitively, a learner with low planning regret can accurately predict the trajectories of her chosen policies, even if she may not be able to certify the optimality of those policies.
We show that in the absence of further assumptions, planning regret can scale linearly in the time horizon, even when the separation between the two systems is a hyperplane. We then show that, when the dynamics have a small amount of stochastic noise, there is an algorithm which enjoys sublinear planning regret, and makes at most polynomially-many calls to an ERM oracle for piecewise affine regression. Our work uncovers new connections between system identification and smoothed online learning which we hope will prove useful as the learning-for-control community sets its sights beyond LTI system identification. 
This is joint work with Adam Block, Sasha Rakhlin, and Russ Tedrake at MIT. 
  
  **Biography:** Max Simchowitz is a postdoctoral researcher under Russ Tedrake in the Robot Locomotion group, part of CSAIL at MIT. He received his PhD in the EECS department at UC Berkeley under Michael I. Jordan and Benjamin Recht, generously supported by Open Philanthropy, NSF GRFP, and Berkeley Fellowships, and was fortunate enough to receive a ICML best paper award. His work focuses broadly on machine learning theory, with a recent focus on the plentiful intersections between statistical learning theory, online learning, non-convex optimization, and control theory. 
</details>



<details>
  <summary> 
    <i>Learning with little mixing</i>, <strong>Ingvar Ziemann (KTH)</strong> </summary>
  <br>
  
  **Abstract:** We study square loss in a realizable time-series framework with martingale difference noise. Our main result is a fast rate excess risk bound
which shows that whenever a
*trajectory hypercontractivity* condition holds,
the risk of the least-squares estimator on dependent data matches the 
iid rate order-wise after a burn-in time.
This is in stark contrast to existing results in learning from dependent data, where
the effective sample size is deflated by a factor of the mixing-time of the underlying process,
even after burn-in.
Furthermore, our results allow the covariate process to exhibit long range correlations,
and do not require geometric ergodicity.
We call this phenomenon *learning with little mixing*.
Several examples are presented for which this phenomenon occurs: 
bounded function classes for
which the $L^2$ and $L^{2+\epsilon}$ norms are equivalent, 
finite state irreducible and aperiodic Markov chains,
and a broad family of infinite dimensional function classes 
based on subsets of $\ell^2(\mathbb{N})$ ellipsoids.
The key technical development is in using trajectory hypercontractivity to show 
that empirical $L^2$ lower isometry holds with only a mild dependence on the mixing-time
of the data generating process.
This is joint work with Stephen Tu.   
  
  **Biography:** Ingvar Ziemann is a PhD student at KTH supervised by Henrik Sandberg. His work focuses on the statistical and information-theoretic aspects of learning-enabled control. Before starting his PhD studies he obtained two sets of Master's and Bachelor's degrees in Mathematics (SU/KTH) and in Economics and Finance (SSE).  
</details>


<details>
  <summary> 
    <i>Provable Regret Bounds for Deep Online Learning and Control</i>, <strong>Xinyi Chen (Princeton)</strong> </summary>
  <br>
  
  **Abstract:** The use of deep neural networks has been highly successful in reinforcement learning and control, although few theoretical guarantees for deep learning exist for these problems. There are two main challenges for deriving performance guarantees: a) control has state information and thus is inherently online and b) deep networks are non-convex predictors for which online learning cannot provide provable guarantees in general.
Building on the linearization technique for overparameterized neural networks, we derive provable regret bounds for efficient online learning with deep neural networks. First we define an expressivity notion that is suited for agnostic and online deep learning. We then show that over any sequence of convex loss functions, any low-regret algorithm can be adapted to optimize the parameters of a neural network such that it competes with the best net in hindsight.  As an application, we obtain provable bounds for online and episodic control with deep neural network controllers.  
  
  **Biography:** Xinyi Chen is a PhD candidate in the Department of Computer Science at Princeton University advised by Prof. Elad Hazan. She is also affiliated with Google AI. Previously, she obtained her undergraduate degree from Princeton in Mathematics, where she received the Middleton Miller Prize. She is a recipient of the NSF Graduate Research Fellowship and a participant of EECS Rising Stars at UC Berkeley. 
</details>

<details>
  <summary> 
    <i>Identification and Control of Multiple Unknown Linear Systems</i>, <strong>Mohamad Kazem Shirani Faradonbeh (University of Georgia)</strong> </summary>
  <br>
  
  **Abstract:** Identification of multiple related linear systems and joint adaptive control policies for them, are problems of interest that remain unexplored to date. We develop a joint estimator of the transition matrices of multiple systems that share common basis matrices and establish finite-time bounds that reflect the influence of trajectory lengths, dimension, number of systems, and the transition matrices. The results are general and showcase the gains from pooling data across systems, in comparison to individual system identifications. We also discuss joint adaptive stabilization algorithms for stabilizing all systems, using the data of unstable state trajectories. An effective algorithm will be presented that stabilizes the family of dynamical systems in a short time period.  
  
  **Biography:** Mohamad Kazem Shirani Faradonbeh is an assistant professor of Data Science in the Department of Statistics at the University of Georgia. During Fall 2020, he was a fellow of Theory of Reinforcement Learning program in Simons Institute for the Theory of Computing at the University of California - Berkeley. Before that, he was a postdoctoral research associate with the Informatics Institute and with the Department of Statistics at the University of Florida. He received PhD in statistics from the University of Michigan, Ann Arbor in 2017, and BSc in electrical engineering from Sharif University of Technology, Tehran, Iran, in 2012.  
</details>

<details>
  <summary> 
    <i>Identification and Adaptive Control of Markov Jump Systems</i>, <strong>Samet Oymak (UC Riverside)</strong> </summary>
  <br>
  
  **Abstract:** 
Learning how to effectively control unknown dynamical systems is crucial for intelligent autonomous systems. This task becomes a significant challenge when the underlying dynamics are changing with time. Motivated by this challenge, in this talk, we discuss the problem of controlling an unknown Markov jump linear system (MJS) to optimize a quadratic objective. By taking a model-based perspective, we follow an identification-based adaptive control strategy. We first provide a system identification algorithm to learn the dynamics in each mode as well as the Markov transition matrix, underlying the evolution of the mode switches, from a single trajectory, and establish associated statistical guarantees. We then propose an adaptive control scheme that performs system identification together with certainty equivalent control to adapt the controllers in an episodic fashion. Combining our sample complexity results with MJS perturbation results for certainty equivalent control, we show that when the episode lengths are appropriately chosen, the proposed adaptive control scheme achieves $O(\sqrt(T))$ regret, which can be improved to $O(polylog(T))$ with partial knowledge of the system. Finally, we provide a discussion of technical innovations to handle Markovian jumps and mean-square stability as well as insights into system theoretic quantities that affect learning accuracy and control performance.
  
  
  **Biography:** Samet Oymak is an assistant professor of Electrical and Computer Engineering at the University of California, Riverside. During his postdoc, he was at UC Berkeley as a Simons Fellow and a member of AMPLab. He obtained his bachelor's degree from Bilkent University in 2009 and PhD degree from Caltech in 2015. At Caltech, he received the Charles Wilts Prize for the best departmental thesis. At UCR, he received an NSF CAREER award as well as a Research Scholar award from Google.
[Website](https://intra.ece.ucr.edu/~oymak/) 
</details>


