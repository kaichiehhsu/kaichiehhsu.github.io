---
title: 		"General Examination Abstract"
collection:	posts
permalink: 	/posts/general
date: 		2021-03-17
---

<center>
	<a href="/files/generalExam.pdf" target="_blank" class="btn btn-danger">
		<span style="font-size: 120%;">
		    Slides
		</span>
	</a>
</center>

Recent developments in deep reinforcement learning have shown promising results to improve the capabilities of autonomous systems. However, for safety-critical robotic systems, it is crucial to provide safety and liveness certificates around these data-driven methods. I focus on three fundamental challenges:
1. how to guarantee systems can reach certain goal conditions while staying clear of unacceptable failure modes, which is known as reach-avoid control problems,
2. how to provide safety and convergence guarantees for learning-based multi-agent reinforcement learning in zero-sum games, and
3. how to infer and distinguish soft and hard constraints in human preferences by using their ranking feedback.

In this examination, I first present my recent work, where I used **deep reinforcement learning to solve reach-avoid optimal control problems** in a range of nonlinear systems. I derived a time-discounted reach-avoid Bellman equation and then proved that the corresponding reach-avoid Q-learning converges, and the resulting reach-avoid sets formed a convergent family of conservative approximations. My next steps will be to use learned reach-avoid solutions to provide a recursively feasible guarantee in a supervisory control scheme. Also, I will extend the proposed framework to partially observable environments, e.g., finite sensing radius, and investigate whether guarantees still hold.

A second direction I have begun to explore is using the proposed reach-avoid Q-Learning in an **attack-defense game**. I had two exciting observations: (1) a sub-optimal defender makes the attacker unable to catch the worst adversarial policies, and (2) there are weak spots in neural network control policies such that the defender can exploit unintuitive and sub-optimal behaviors to ``fool'' the attacker. In the future, I want to look into if the principle of iterative adversarial improvements leads to a convergent training process and explore how malicious actions from other agents influence learning-based policies.

Finally, in the **inverse specification** project, I used Bayesian optimization to infer constraints interactively with humans by asking for ranking feedback on multiple candidate solutions. I showed that by actively selecting queries with better information-theoretic metrics, the belief converges faster to the actual state. It is indispensable to distinguish hard constraints from soft constraints (or cost components in the overall objective function). My future work is to select queries to discriminate hard and soft constraints and formulate efficient potential constraint sets. I will incorporate this method into a cyber-physical system co-design framework, where designers and the machine work together to explore the design space efficiently.


### Reading List
1. J. F. Fisac, M. Chen, C. J. Tomlin, and S. S. Sastry. “Reach-Avoid Problems with Time-Varying Dynamics, Targets and Constraints”. Proceedings of the 18th International Conference on Hybrid Systems: Computation and Control. HSCC ’15. Seattle, Washington: Association for Computing Machinery, 2015, pp. 11–20.
2. J. F. Fisac, N. F. Lugovoy, V. Rubies-Royo, et al. “Bridging Hamilton-Jacobi Safety Analysis and Reinforcement Learning”. 2019 International Conference on Robotics and Automation (ICRA). 2019, pp. 8550–8556.
3. J. F. Fisac, A. K. Akametalu, M. N. Zeilinger, et al. “A General Safety Framework for Learning-Based Control in Uncertain Robotic Systems”. IEEE Transactions on Automatic Control 64.7 (2019), pp. 2737–2752.
4. O. Bastani. “Safe Reinforcement Learning with Nonlinear Dynamics via Model Predictive Shielding”. 2020. arXiv: 1905.10691 [cs.LG].
5. B. D. Ziebart, A. L. Maas, J. A. Bagnell, and A. K. Dey. “Maximum Entropy Inverse Reinforcement Learning”. Proceedings of the 23rd National Conference on Artificial Intelligence. AAAI. 2008.
6. J. Ho and S. Ermon. “Generative Adversarial Imitation Learning”. Advances in Neural Information Processing Systems. Ed. by D. Lee, M. Sugiyama, U. Luxburg, et al. Vol. 29. Curran Associates, Inc., 2016, pp. 4565–4573.
7. D. R. Scobee and S. S. Sastry. “Maximum Likelihood Constraint Inference for Inverse Reinforcement Learning”. International Conference on Learning Representations. 2020.
8. D. Hadfield-Menell, S. Milli, P. Abbeel, et al. “Inverse Reward Design”. Advances in Neural Information Processing Systems. 2017, pp. 6765–6774.
9. D. Hadfield-Menell, S. J. Russell, P. Abbeel, and A. Dragan. “Cooperative inverse reinforcement learning”. Advances in neural information processing systems. 2016, pp. 3909–3917.
10. J. F. Fisac, M. A. Gates, J. B. Hamrick, et al. “Pragmatic-pedagogic value alignment”. Robotics Research. Springer, 2020, pp. 49–57.
11. P. Christiano, J. Leike, T. B. Brown, et al. “Deep reinforcement learning from human preferences” (2017). arXiv: 1706.03741 [stat.ML].
12. J. Heinrich, M. Lanctot, and D. Silver. “Fictitious Self-Play in Extensive-Form Games”. Proceedings of the 32nd International Conference on Machine Learning. Vol. 37. Proceedings of Machine Learning Research. Lille, France: PMLR, July 2015, pp. 805–813.
13. R. Lowe, Y. WU, A. Tamar, et al. “Multi-Agent Actor-Critic for Mixed Cooperative-Competitive Environments”. Advances in Neural Information Processing Systems. Ed. by I. Guyon, U. V. Luxburg, S. Bengio, et al. Vol. 30. Curran Associates, Inc., 2017.
14. J. Foerster, G. Farquhar, T. Afouras, et al. “Counterfactual Multi-Agent Policy Gradients”. Proceedings of the AAAI Conference on Artificial Intelligence 32.1 (Apr. 2018).