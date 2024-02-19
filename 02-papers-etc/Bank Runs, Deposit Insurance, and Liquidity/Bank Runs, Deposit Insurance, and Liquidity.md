# Title: Bank Runs, Deposit Insurance, and Liquidity
##### Author(s): Douglas W. Diamond, Philip H. Dybvig
##### Year: 1983
##### Journal: *Journal of Political Economy*

Abstract: This paper shows that bank deposit contracts can provide allocations superior to those of exchange markets, offering an explanation of how banks subject to runs can attract deposits. Investors face privately observed risks which lead to a demand for liquidity. Traditional demand deposit contracts which provide liquidity have multiple equilibria, one of which is a bank run. Bank runs in the model cause real economic damage, rather than simply reflecting other problems. Contracts which can prevent runs are studied, and the analysis shows that there are circumstances when government provision of deposit insurance can produce superior contracts.

URL/DOI: https://doi.org/10.1086/261155

### Research question:
- Why do bank runs occur and what can be done to stop them?

### Data:

### Relevant Literature:
- Friedman and Schwartz (1963) did some study of properties of bank runs in the US (particularly in the depression?)
	- See [[]]
- Bernanke (1983) on Great Depression Bank Runs
	- See [[]]
- On the liquidity of assets: Patinkin (1965, chapter 5), Tobin (1965), Niehans (1978)
	- See [[]]
	- See [[]]
	- See [[]]
- Empirical evidence on whether deposit insurance reduces the likelihood of failure:
	- Merton (1977) See [[]]
	- Merton (1978) See [[]]
	- Kareken  and Wallace (1978) See [[]]
	- Dothan and Williams (1980) See [[]]

### Hypothesis and setup:
- In this model, banks are not just intermediaries. "Existing theoretical analysis has neglected to explain why bank contracts are less table than other types of financial contracts or to investigate the strategic decisions that depositors face. The model we present has an explicit economic role for banks to perform: the transformation of illiquid assets into liquid liabilities."
	- "Uninsured demand deposit contracts are able to provide liquidity but leave banks vulnerable to runs. This vulnerability occurs because there are multiple equilibria with differing levels of confidence."
	- Agents hold private information about their desire to allocate wealth over time (and information states). Because this private information cannot be observed by other parties, general insurance contracts cannot be written for this information space: hence the need for a bank.
	- "Banks are able to transform illiquid assets by offering liabilities with a different, smoother pattern of returns over time than the illiquid assets offer. These contracts have multiple equilibria"
		- "If confidence is maintained, there can be efficient risk sharing, because in that equilibrium a withdrawal will indicate that a depositor should withdraw under optimal risk sharing. if agents panic, there is a bank run and incentives are distorted. In that equilibrium, everyone rushes in to withdraw their deposits before the bank gives out all of its assets. The bank must liquidate all of its assets, even if not all depositors withdraw, because liquidated assets are sold at a loss."
	- "In contrast, a bank run in our model is caused by a shift in expectations, which could depend on almost anything, consistent with the apparently irrational observed behavior of people running on banks."
- "Our model demonstrates three important points:"
	1. "First, banks issuing demand deposits can improve on a competitive market by providing better risk sharing among people who need to consume at different random times."
	2. "Second, the demand deposit contract providing this improvement has an undesirable equilibrium ( a bank run), in which all depositors panic and withdraw immediately, including even those who would prefer to leave their deposits in if they were not concerned about the bank failing."
	3. "Third, bank runs cause real economic problems because even 'healthy' banks can fail, causing the recall of loans and the termination of productive investment."
- "In addition, our model provides a suitable framework for analysis of the devices traditionally used to stop or prevent bank runs, namely, suspension of convertibility and demand deposit insurance (which works similarly to a central bank servings as 'lender of last resort')."
- Alone, banks offering suspension-of-convertibility contracts does not achieve optimal risk sharing.
- "Deposit insurance is shown to be able to rule out runs without reducing the ability of banks to transform assets."
	- Deposit insurance "frees the asset liquidation policy from strict dependence on the volume of withdrawals"
- Other options: the discount window at a central bank
### Headline results:

**The Bank's Role in Providing Liquidity**
- The model has three periods: $T =0,1,2$
- A single homogenous good is produced 
	- At period $T=0$ a single such unit can be used as an input in production technology which generates $R>1$ at $T=2$ in the case that production completes. Otherwise, if production is interrupted at $T=1$, it returns $1$.
	- CRS is possible so $R>1$ is a weak constraint. 
	- The effective choice is between $(0,R)$ and $(1,0)$, which must be decided up on at $T=1$
	
| $T=0$ |  | $T=1$ | $T=2$ |
| ---- | ---- | ---- | ---- |
| -1 | Production is completed | 0 | R |
|  | Production is interrupted | 1 | 0 |
- This technology corresponds to long-term capital investments being somewhat irreversible.
	- In the parlance of a bank, this can be mapped on to "any type of transaction cost associated with selling a bank's assets before maturity. See Diamond (1980) for a model of the costly monitoring of loan contracts by banks, which implies such a cost." 
		- See [[]]
- Consumers
	- All are identical at period 0. All agents can be assigned a type characterizing uninsurable risk (type 1 or type 2), privately observed at $t=1$.
		- Type 1 agents care only about consumption at $T=1$,
		- Type 2 agents care only about consumption at $T=2$.
	- All agents have ability to privately store/hoard the good. No one would do so between $T=0$ and $T=1$ because the productive technology does at least as well (for type 1) and better (for type 2)
	- $$ U(c_1, c_2; \Theta) = \begin{cases} 
		  u(c_1) & \text{if $j$ is of type 1 in state $\Theta$} \\
		  \rho u(c_1, + c_2) & \text{if $j$ is of type 2 in state $\Theta$}
	\end{cases}$$
		- $1 \geq \rho > R^{-1}$
		- $u: \mathbb{R}_{++}\to \mathbb{R}$ is twice continuously differentiable, increasing, strictly concave, and satisfies the Inada conditions
			- The coefficient of relative risk aversion is $-cu''(c)/u'(c)>1$ everywhere
		- Agents maximize expected utility, conditional on their information
		- Agent types are assigned independently and identically.
		- A fraction $t \in (0,1)$ of agents are type 1. For now this is a constant (later this will be relaxed to be constant)
	- Agents are endowed with unit of the good at $T=0$.
	- Direct Contracting Competitive Solution (ADE)
		- Price of period-1 goods is $1$
		- Price of period-2 goods is $1/R$ 
		- Because agent's do know each others types. There is no public information to condition the contracts on.
			- This produces zero 0 trade.
		- *IF* types were publicly observable "it would be possible to write optimal insurance contracts that give the ex ante (as of period 0) optimal sharing of output between type 1 and type 2 agents". This yields allocations
			- $$c_1^{2*} = c_2^{1*} =0 \tag{1a}$$(agent type-superscript doesn't care about consumption in period-subscript)
			- $$u'(c_1^{1*})= \rho R u'(c_2^{2*}) \tag{1b}$$ (those who can, delay consumption to the second period and marginal utilities are equal to the marginal productivity)
				- Note that $c_2^{2*} > c_1^{1*}$ as $\rho R > 1$.
			- $$tc_1^{1*} +(1-t)(c_2^{2*}/R)=1\tag{1c}$$ (the resource constraint.)
			- By definition $\rho R >1$ "and since relative risk aversion always exceeds unity, equation (1) implies that the optimal consumption levels satisfy $c_1^{1*}$ and $c_2^{2*}< R$. Therefore, there is room for improvement on the competitive outcome (where $c_1^1 = 1, c_2^2=R$)"
	- Demand Deposit Contracts
		- Gives each agent withdrawing in period 1 a fixed claim of $r_1$ per unit deposited at time $T=0$.
			- "Withdrawal tenders are served sequentially in random order until the bank runs out of assets. This approach allows us to capture the flavor of continuous time (in which depositors deposit and withdraw at different random times) in a discrete model."
			- "Note that the demand deposit contract satisfies a *sequential service constraint*, which specifies that a bank's payoff to any agent can depend only on the agent's place in line and not on future information about agents behind him in line."
				- The bank is mutually owned and liquidated in period 2 "so that agents not withdrawing in period 1 get a pro rata share of the bank's assets in period 2".
			- $$V_1(f_j,r_1) = \begin{cases}
				  r_1 & \text{if $f_j < r_1^{-1}$}\\
				  0 & \text{if $f_j \geq r_1^{-1}$}
			  \end{cases} \tag{2}$$
			  - $V_1$ is the period 1 payoff per unit deposit withdrawn (which depends on position in line)
			  - $$v_2(f, r_1) = \max\{\frac{R(1-r_1f)}{1-f}, 0\} \tag{3}$$
			  - $V_2$ is the period 2 payoff per unit deposit *not* withdrawn at $T=2$ (ie after liquidation?)
			  - $f_j$ is the number of withdrawer's deposited before agent $j$ (as a fraction of total demand deposits).
			  - $f$ is the total number of demand deposits withdrawn.
			  - Consumption generated from agent $j$'s withdrawals can thus be specified as
				  - Type 1: $w_jV_1(f_j,r_1)$
				  - Type 2: $w_jV_1(f_j, r_1)+ (1-w_j)(V_2(f, r_1))$
				  - where $w_j$ is the share of of agent $j$'s deposits of which withdrawals are attempted at $T=1$
		  - *Equilibrium decisions*
			  - We restrict attention to pure strategy Nash equilibria
			  - The full-information, optimal risk sharing setting is achievable as an equilibrium with the demand deposit contract
				  - This occurs when $r_1 = c_1^{1*}$, so that fixed payment per dollar of deposits withdrawn at $T=1$ is equal to the optimal consumption of a type 1 agent given full information.
					  - Type 2 agents will wait.
			  - The "bank run" equilibrium also arises:
				  - If agents believe that this is the equilibrium, then they all want to withdraw at $T=1$.
					  - "This is because the face value of deposits is larger than the liquidation value of the bank's assets" (so Type 2 agents have no incentive to wait - they can withdraw and use the hoarding technology)
				  - For all $r_1 >1$ runs are equilibrium
				  - For $r_1 =1$ the bank technology is identical to the simple competitive claims market. 
					  - $V_1(f_j, 1) < V_2(f_j,1)$ for all $0 \leq f_j \leq f$.
					  - "A demand deposit contract which is not subject to runs provides no liquidity services"
					  - But observe that this run equilibrium has risk whereas the personal-holding technology is riskless (and offers a return greater than 1, $R>1$, if you turn out to be an agent of Type 2)
				  - "If we take the position that outcomes must match anticipations, the inferiority of bank runs seems to rule out observed runs, since no one would deposit anticipating a run. However, agent will choose to deposit at least some of their wealth in the bank even if they anticipate a positive probability of a run, provided that the probability is small enough, because the good equilibrium dominates holding assets directly. This could happen if the selection between the bank run equilibrium and the good equilibrium depended on some commonly observed random variable. in the economy. This could be a bad earnings report, a commonly observed run at some other bank, a negative government forecast, or even sunspots. It need not be anything fundamental about the bank's condition. The problem is that once they have deposited, anything that causes them to anticipate a run will lead to a run. This implies that banks with pure demand deposit contracts will be very concerned about maintaining confidence because they realize that the good equilibrium is very fragile."
			  
**Improving on Demand Deposits: Suspension of Convertibility**
- If banks can suspend convertibility when attempted withdrawals at $T=1$ are too numerous:
	- This could convince Type 2 agents to wait rather than withdraw early.
	- But some Type 1 agents will not be able to make early withdrawals if they show up too late.
	- So we redefine $(2)$ and $(3)$ as
		- $$V_1(f_j, r_1) = \begin{cases}
			  r_1 & \text{if $f_j \leq \hat{f}$}\\
			  0 & \text{if $f_j > \hat{f}$}
		  \end{cases}$$
		  - convertibility is suspended when $f_j = \hat{f}$.
		  - $$V_2(f,r_1) = \max\{\frac{(1-fr_1)R}{1-f}, \frac{(1-\hat{f}r_1) R}{1-\hat{f}}\}$$
			  - where $V_2$ assumes that $1- \hat{f}r_1 >0$
  - This can replicate optimal risk sharing if $r_1 = c_1^{1*}$ and for any $\hat{f} \in \{t, \frac{R-r_1}{r_1(R-1)}\}$.
	  - Type 2 agents don't try to withdraw at $T=1$ because they are guaranteed consumption at $T=2$
		  - For all $f$ and $f_j \leq f$ $V_2(\cdot) > V_1(\cdot)$
	  - Type 1 agents all try to make withdrawals at $T=1$ because for them $T=2$ consumption goods are worthless.
	  - "Therefore there is a unique Nash equilibrium which has $f=t$. In fact, this is a dominant strategy equilibrium, because each agent will choose his equilibrium action even if he anticiaptes that other agents will choose his nonequilbrium or even irrational actions. This makes this contract very 'stable.'"
		  - "This contract works perfectly only in the case where the normal volume of withdrawals, $t$, is known and not stochastic. The more general case, where $t$ can vary, is analyzed next"

**Optimal Contracts with Stochastic Withdrawals**
- Now we suppose that the distribution of types $t$ is an unknown/unobserved random variable: $\tilde{t}$
	- Recall in $(1)$ we are able to describe the (optimal) equilibrium condition as non-consumption in irrelevant periods.. We can restate that in this setting as
		- $$c_2^{1*}(t) = c_1^{2*}(t) = 0$$
			- "This implies a unique optimal asset liquidation policy given $\tilde{t}=t$. This turns out to imply that uninsured bank deposit contracts cannot achieve optimal risk sharing."
- PROPOSITION 1: "Bank contracts (which must obey the sequential service constraint) cannot achieve optimal risk sharing when $t$ is stochastic and has a nondegenerate distribution."
	- "We prove that no bank contract can attain the full-information optimal risk sharing. The proof is straightforward, a two-party proof by contradiction."
		- "place in line" can be expressed by $f_j$ which is distributed uniformly over $[0,t]$ if only Type 1 agents attempt withdrawals.
		- "First, suppose that the payments to those who withdraw at $T=1$ is a nonconstant function of $f_j$ over feasible values of $t$: for two possible values of $\tilde{t}$, $t_1,$ and $t_2$, the value of a period 1 withdrawal varies, that is $V_1(t_1)\neq V_1(t_2)$. This immediately implies that there is a positive probability of different consumption levels by two type 1 agents who will withdraw at $T=1$, and this contradicts an unconstrained optimum. Second, assume the contrary: that for all possible realizations of $\tilde{t} =t$, $V_1(f_j)$ is constant for all $f_j \in [0,1]$. This implies that $c_1^1(t)$ is a constant independent of the realization of $\tilde{t}$, while the budget constraint, equation (1c), shows that $c_2^2(t)$ will vary with $t$ (unless $r_1=1$ ... Constant $c_1^1(t)$ and varying $c_2^2(t)$ contradict optimal risk sharing, equation (1b). Thus optimal risk sharing is inconsistent with sequential service."
	- The problem comes from the point $\hat{f}$ being less than the largest possible realization of $\tilde{t}$.
		- I.e. some Type 1 agents will not be able to make withdrawals, which is inefficient ex post.
		- Ex ante, the threat of suspension is desirable "because the threat of suspension prevents runs and allows a relatively high value of $r_1$."

**Government Deposit Insurance**
- The proposed deposit insurance permits contracts that "dominate the best that can be offered without insurance and never do worse."
	- The model is kept closed and aggregate resource constraints are not violated.
	- In theory it could be possible to make this a private entity but pragmatically it makes sense for it to be administered by the government.
- The government can levy a tax on agents who withdraw at $T=1$ (ie those with low $f_j$)
	- The amounts raised depends on the share of deposits withdrawn, $f_j$, and the promised/permitted withdrawals at $T=1$, $r_1$.
		- If every deposit were withdrawn at $T=1$ (i.e. $f=1$) and $r_1=2$ were promised, "a tax of at least one per capita would need to be raised because totally liquidating the bank's assets will raise at most one per capita at $T=1$. As the government can impose a tax on an agent *after* he or she has withdraw, the government can base its tax on $f$, the realized total value of $T=1$ withdrawals."
			- Governments are different from banks because banks are required to satisfy the sequential service constraint and cannot reduce the size of the withdrawal after it has been made, whereas the government need not adhere to this.
			- Agents are concerned with maximizing after-tax value of consumption.
- PROPOSITION 2: "Demand deposit contracts with government deposit insurance achieve the unconstrained optimum as a unique Nash equilibrium (in fact, a dominant strategies equilibrium) if the government imposes an optimal tax to finance the deposit insurance."
	- Say governments levy the tax at the beginning of period $T=1$ payable either in goods or in deposits.
	- "Consider the proportionate tax as a function of $f, \tau: [0,1] \to [0,1]$ given by"
		- $$\tau(f) = \begin{cases}
			  1- \frac{c_1^{1*}-f}{r_1} & \text{if $f \leq \bar{t}$}\\
			  1 - \frac{1}{r_1} & \text{if $f > \bar{t}$},
		  \end{cases}$$
		  - where $\bar{t}$ is the greatest possible realization of $\tilde{t}$
	  - Type 1-agent after-tax proceeds are given by $\hat{V}_1$
		  - $$\hat{V}_1 = \begin{cases}
			    c_1^{1*} & \text{if $f \leq \bar{t}$}\\
			    1 & \text{if $f > \bar{t}$}
		    \end{cases}$$
	- "The net payments to those who withdraw at $T=1$ determine the asset liquidation policy and after-tax value of a withdrawal at $T=2$. Any tax collected in excess of that needed to meet withdrawals at $T=1$ is plowed back into the bank (to minimize the fraction of assets liquidated.) This implies that the the after-tax proceeds, per dollar of initial deposit, of a withdrawal at $T=2$, denoted by $\hat{V}_2(f)$ are given by"
	- $$\hat{V}_2(f) = \begin{cases}
	  \frac{R(1-c_1^{1*}(f)f)}{1-f} &= c_2^{2*}(f) & \text{if $f \leq \bar{t}$}\\
	  \frac{R(1-f)}{1-f} &= R  & \text{if $f > \bar{t}$}
	  \end{cases}$$
	  - $\hat{V}_1(f) < \hat{V}_2(f)$ for all $f\in [0,1]$ so no agents of Type 2 will attempt a withdrawal at $T=1$
	  - For all $f\in[0,1]$ $\hat{V}_1(f)>0$, implying that all Type 1 agents will withdraw at $T=1$.
	  - "Therefore, the unique dominant strategy equilibrium if $f=t$, the realization of $\tilde{t}$. Evaluated at a realization $t$,"
		  - $$\hat{V}_1(f=t) = c_1^{1*}(t$$
		  - and
		  - $$\hat{V}_2(f=t) = \frac{[1-tc_1^{1*}(t)]R}{1-t} = c_2^{2*}(t)$$
		  - And the optimum is achieved
  - This result riles on the government being able to levy a non-distortionary tax. 
  - "Deposit insurance can be provided costlessly in the simple case where $t$ is nonstochastic, for the same reason that there need not be a suspension of convertibility in equilibrium. The deposit insurance guarantees that type 2 agents will never participate in a run; without runs, withdrawals are deterministic and this feature is never used. In particular, so long as the government can impose *some* tax to finance the insurance, no matter how distortionary, there will be no runs and the distorting tax need never be imposed. This feature is shared by a model of adoption externalities (See Dybvig and Spatt, [1983]), in which a Pareto-inferior equilibrium can be averted by an insurance policy which is costless in equilibrium."
	  - See [[]]
### Important figures/viz:

### Important figures/viz:

### Concepts, models & tags:
- #Author/DouglasWDiamond
- #Author/PhilipHDybvig
- #Financial_Economics 
- #Banking

### BibTeX and other citation information:
- **As it should appear in Chicago:** Diamond, Douglas W., and Philip H. Dybvig. "Bank runs, deposit insurance, and liquidity." *Journal of Political Economy* 91, no. 3 (1983): 401-419.
- **BibTeX key:** @article{diamond1983bank,
  title={Bank runs, deposit insurance, and liquidity},
  author={Diamond, Douglas W and Dybvig, Philip H},
  journal={Journal of Political Economy},
  volume={91},
  number={3},
  pages={401--419},
  year={1983},
  publisher={The University of Chicago Press}
}