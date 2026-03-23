Binomial Proportion:
	If the Binomial Conditions are satisfied, then the proportion of 'successes' out of the draw of $n$ observations is said to be Binomial with constants $n$ and $p$, and is computed as:
		$\hat{P} = \frac{\text{number of success in sample}}{n}$
The Sampling Distribution of sample proportion Pˆ :
	If a sample is selected, and if a Binomial categorical variable is recorded for each individual:
		if a fixed sample size n was selected, and if each individual sampled is either ‘success’ or ‘failure’,
		and if the sample is from a population with fixed proportion p of ‘success’,
		 and if the sample was selected at random, and if the sampling was with replacement or else from a population that is relatively large compared to the sample size (like, at least 20 times as large),
	then the distribution of sample proportion pˆ has the following features:
		Center:
			mean of sample proportions = population proportion .
			$\mu_\hat{p} = p$ 
		Spread:
			$\sigma_\hat{p} = \sqrt{\frac{(p)(1-p)}{n}}$
			(This is valid as long as the outcomes are independent (i.e., if sampling with replacement, or else if the population is relatively large compared to the sample)
		Shape:
			(Central Limit Theorem for Proportions):
				If $np$ and $n(1-p)$ are both $\ge 10$, then the $\hat{P}$ distribution is approximately normal
				and the sampling distribution of pˆ is closer to Normal in shape with larger sample size