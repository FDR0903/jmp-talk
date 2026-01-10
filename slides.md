---
layout: cover
class: text-center
title: Design & Incentives in Blockchain Financial Systems
#theme: academic
titleTemplate: '%s'
favicon: ./images/defiicon.png
author: Fayçal Drissi
themeConfig:
  paginationX: disabled
  paginationY: disabled
  paginationPagesDisabled: [1]
fonts:
  local: Montserrat, Roboto Mono, Roboto Slab # local fonts are used for legal reasons for deployment to https://slidev-theme-academic.alexeble.de and only set up for the example project, remove this line for your project to automatically have fonts imported from Google

theme: frankfurt
infoLine: true # on by default, can be turned off
#author: 'Your name here' # shows in infoLine
#title: 'Title' # shows in infoLine
date: '14/12/2025' # shows in infoLine, defaults to the current date

mdc: true
---

## These slides:  [faycaldrissi.com/staking_talk/](https://www.faycaldrissi.com/staking_talk/)

<br>

# Design and Incentives in Blockchain Financial Systems

## Fayçal Drissi

### *University of Oxford*
<br>

<!--These slides: [https://www.faycaldrissi.com/siam2025](https://www.faycaldrissi.com/siam2025)
[my scholar](https://scholar.google.com/citations?user=njvyriQAAAAJ&hl=fr), 
[my website](https://www.faycaldrissi.com/), [my github](https://github.com/FDR0903)-->

---
section: Blockchains
---

# Decentralised financial systems

### Modern economies rely on trusted intermediaries (banks, clearing houses, platforms, governments)
- Intermediaries reduce transaction and enforce contracts, but introduce
  - fees, delays, opacity, 
  - market power, exclusion, censorship risk

<br>

### Central question: Can we coordinate economic activity at scale with less centralized trust?

- Blockchains are a technological and economic response to trust, coordination, and institutional frictions
  - Shared, tamper-resistant ledger
  - Maintained by algorithmic rules (consensus) and incentives, not a single authority
  - general-purpose infrastructure for economic coordination, replaces institutional trust with 
    - publicly verifiable rules
    - economic incentives: participants are rewarded to follow rules


---


# Decentralised financial systems

### Decentralised finance (DeFi) as a new form of financial intermediation
- DeFi = financial services run by smart contracts on blockchains
  - Open access
  - Automated execution   
  - No centralized balance sheet
- Intermediation becomes a **protocol**
- Contracts enforced by code + incentives, not courts
<br><br>

### Breadth of real economic applications
- Payments & Money: Stablecoins, Cross-border payments
- Financial Markets: Decentralized exchanges, On-chain lending,  collateralized credit
- Organizations & Governance: DAOs (Decentralized Autonomous Organizations)
  - Firms or collectives governed by token-holders
  - Rules for voting, treasury use, and upgrades are pre-specified
- Ownership/contracting: financial and real asset tokenisation

---


# My research

- Blockchain technology for ...

---
section: Market Microstructure
layout: center
---

**Agostino Capponi, Alvaro Cartea, Fayçal Drissi (2025). Do Longer Block Times Impair Market Efficiency in Decentralized Markets?**

<center> 
Columbia University, University of Oxford

**Link**:  [faycaldrissi.com/files/mempools.pdf](https://www.faycaldrissi.com/files/mempools.pdf)
</center>

---

# Motivation


- Significant volumes on Decentralized Exchanges (DEXs): ($\$7.383$ billion in $24$ hours) as of 7 May 2025
  
  $\implies$ DEX efficiency actively influences discussions on blockchain design

<v-click>

- The blockchain protocol determines the lifecycle of transactions and adds new cost structures

<v-click>

- Transactions are sent to the network continuously, stored in a memory pool. At each Epoch, with length **block time**, a validator is chosen. The validator creates a new block with transactions from the memory pool

![blockchain1](./images/blockchaincreation1.png){style="transform: translate(20%, 0%); width: 580px"}

<v-click>

![blockchain1](./images/blockchaincreation2.png){style="transform: translate(20%, -102%); width: 580px"}

<v-click>

![blockchain1](./images/blockchaincreation3.png){style="transform: translate(20%, -210%); width: 580px"}

</v-click>
</v-click>
</v-click>
</v-click>

---

# Motivation: the blockchain protocol

### Gas fees (EIP-1559)
* **Base fee**: based on congestion, prerequisite for inclusion
* **Priority fee**: incentivise validators to prioritise a transaction in the block $\implies$ Agents compete for queue priority
<v-click>

![mempools](./images/mempools.jpeg){style="transform: translate(25%, 0%); width: 580px"}

</v-click>

---

# Contribution

### A model to describe the microstructure of blockchains financial markets
<u>**stage 0**</u>: $M< L$ traders acquire information for a fixed cost $C$
<br><br>
![model1](./images/model1.png){style="transform: translate(10%, 15%); width: 600px"}
<v-click>
<div style="margin-top:-300px;"> 
<u><b>stage 1</b></u>: liquidity supplier sets the AMM’s reserves
</div>

![model2](./images/model2.png){style="transform: translate(10%, 7%); width: 600px"}
<v-click>

<div style="margin-top:-296px;"> 
<u><b>stage 2</b></u>: M informed traders compete for priority
</div>

![model3](./images/model3.png){style="transform: translate(7.6%, 30%); width: 600px"}

<v-click>

![model4](./images/model4.png){style="transform: translate(10.2%, -78%); width: 600px"}

</v-click>
</v-click>
</v-click>


---

<!--
<br /><br /><br /><br /><br /><br />
<p style="text-align: center;"><h1>
The model is solved by backward induction <a name="defi"></a></h1>
</p>


<br /><br /><br /><br /><br /><br />
<p style="text-align: center;"><h1>
Stage two<br><br>
priority fees and trading volumes <a name="defi"></a></h1>
</p>

-->


# <ins>Stage two</ins>: assumptions

### Competition in each block: multi-prize sealed-bid auction

![distribPF](./images/distribPF.png){style="transform: translate(60.2%, 0%); width: 400px"}

Data: from \textit{EthPandaOps} and it includes $10^7$ transactions observed in the public memory pool of Ethereum between 20~March~2024, 00:00, and 21~March~2024, 17:08

**TODO: Add image that shows that market clears sequentially**

<v-click>

- Informed trader $i\in\{1,\dots,M\}$ has a private and independent type: $v_i=\mathbb{E}_{i}\left[V\right]$ which represents the valuation of the asset
- **In equilibrium of stage two:** traders set the **priority fee $\varphi_i$**, and the **trading volume $\delta_i$** 
</v-click>

---

# <ins>Stage two</ins>

### Informed traders compete to avoid potentially worse execution prices resulting from the adverse price impact of preceding orders in the block

- Execution costs and price impact is approximately linear in the trading volume $\delta$ and inversely proportional to liquidity $\kappa$

$$\footnotesize \text{execution price to buy }\delta = V_0 + \delta / \kappa $$
$$\footnotesize \text{new price following a buy }\delta = V_0 + 2\,\delta / \kappa $$

![convexity1](./images/convexity1.png){style="transform: translate(50%, 0%); width: 450px"}

---

# <ins>Stage two</ins>

- At stage two: number of traders $M$ and liquidity supply $\kappa$ are known
- If trader $i$ is first in the block
$$\scriptsize
W_{i,(M-1)} 
    = \underbrace{-\varphi_i}_\text{priority fee}
    - \underbrace{\delta_i \left( \frac{\delta_i}{\kappa} + \pi \right)}_{\text{cash paid to AMM}}
    + \underbrace{\delta_i \,V}_{\text{terminal value of holdings}}
    - \underbrace{C}_{\text{information cost}}
$$

- If trader $i$ is $j-$th in the block
$$\scriptsize
W_{i,(j)} = {-\varphi_i}
       - \underbrace{\delta_i \!\left( \frac{\delta_i}{\kappa} 
       + \frac{2}{\kappa} \Delta_{(j+1 : M-1)} 
       + \pi \right)}_{\text{exec costs + adverse price impact}}
       + {\delta_i V}
       - {C}
$$

- If trader $i$ is last in the block
$$\scriptsize
W_{i,(0)}
    = -\varphi_{i}
      - \delta_{i}\!\left(
        \frac{\delta_{i}}{\kappa}
        + \frac{2}{\kappa}\,\Delta_{(1:M-1)}
        + \pi
      \right)
      + \delta_{i} V
      - C\,
$$

- **Expected wealth**
$$\scriptsize
\mathbb{E}_{i}\!\left[W_{i}\right]
= \mathbb{E}_{i}\!\left[W_{i,0}\right]
+ \frac{2\,\delta_{i}}{\kappa}
\sum_{j=0}^{M-1}
\mathbb{E}_{i}\!\left[
    \boldsymbol{1}_{\{\varphi_{(j)} < \varphi_{i} < \varphi_{(j+1)}\}}
    \,\Delta_{(1:j)}
\right]
$$

---

# <ins>Stage two</ins>: results
Optimisation problem: $\qquad\qquad\qquad\qquad\qquad\qquad \sup_{\varphi_i, \delta_i} \mathbb{E}_{i}\!\left[W_{i}\right]$

- Participation cutoff: only types $v_i>\underline v_M$ participate, where $\footnotesize
\underline v_M - \pi - \int_{\underline v_M}^{\overline v}\bigl(e^{(1-F(u))(M-1)} - 1\bigr)\,du = 0\,,$ and $\underline v_M(M) \ \ {\nearrow} \ \ \overline v$

![tradingvolumesDist](./images/tradingvolumesDist.png){style="transform: translate(90%, 0%); width: 350px"}

$\implies$ competition decreases informational content in markets

<v-click>

- The equilibrium trading volume: $\quad \footnotesize \delta(v_i) = \kappa\,\tilde \delta(v_i)  = \kappa/2 \left(\left(\overline v - \pi\right)e^{-(M-1)\left(1-F(v_i)\right)} - \int_{v_i}^{\overline v} e^{-(M-1)\left(F(u)-F(v_i)\right)}\,du\right)$

- The equilibrium priority fee: $\qquad\quad \footnotesize \varphi\left(\delta_{i}\right)=\varphi\left(v_{i}\right)=2\,\kappa\left(M-1\right)\int_{\underline{v}_M}^{v_{i}}\tilde{\delta}\left(x\right)^{2}\,f\left(x\right)\,dx\,.$

</v-click>

--- 

# <ins>Stage two</ins>: results

-  $\delta(v_i)$ and $\varphi(v_i)$ are increasing in the private valuation $v_i$: Higher values of private signals correspond to larger trading volumes; they are also associated with higher priority fees and better queue positions. 


![tradingvolumes](./images/tradingvolumes.png){style="transform: translate(90%, 0%); width: 400px"}

Average absolute trading volume of transactions across multiple Uniswap v3 pools as a function of their queue position within the block


- $\delta(v_i)$ and $\varphi(v_i)$ are decreasing in the number of informed traders $M$ with limit 
$$\footnotesize \lim_{M\to\infty}\delta(v_i)=\lim_{M\to\infty}\varphi(v_i)=0.$$


$\implies$ competition decreases individual trading volumes and priority fees However, aggregate trading volumes increase in $M$
$$\footnotesize
\sum_{i=1}^M\,\mathbb E[\tilde \delta(v_i) \mid v_i \ge \underline v_M] = M \, \int_{\underline v_M}^{\overline{v}} \tilde \delta(x) \,dF(x) 
$$


--- 

# <ins>Stages one and zero</ins>
### Stage one: equilibrium liquidity supply
- Liquidity suppliers balance revenue from uninformed elastic demand:
  $$\footnotesize
  \kappa=\sqrt{\frac{\text{revenue}}{M\,S_M}}, \qquad S_M=\int_{\underline v_M}^{\overline v} \tilde\delta(u)^2\,dF(u): \text{ variance of trading volumes} 
  $$
  1. $\footnotesize S_M$ increases with $\footnotesize M$ $\implies$ $\footnotesize \kappa(M)$ decreases with $\footnotesize M$
  2. Market shutdown condition:  $\qquad\qquad\qquad\qquad\footnotesize M\,S_M \le \frac{\text{revenue}}{\text{elasticity}}$

$\implies$ there exists $\overline M$ s.t. for all $M>\overline M$, markets shutdown.

$\implies$ competition is bad for price efficiency **AND** liquidity: in contrast to traditional markets (Holden and Subrahmanyam (1992))

### Stage zero: information acquisition
The number of informed traders is constrained by the profitability of informed trading and the cost $C$
$$\footnotesize
C=\underbrace{\sqrt{\frac{\pi\,N\,\theta}{M\,S_{M}}}\,\int_{\underline{v}_{M}}^{\overline{v}}\left(-2\,\left(M-1\right)\left(S_{M}+\Sigma_{M}\left(v\right)\right)+\tilde{\delta}\left(v\right)\,\left(v-\pi-\tilde{\delta}\left(v\right)\right)\right)dF\left(v\right)}_{H(M) = \text{trading profits net of execution costs and priority fees}}\,,
$$
$\footnotesize M$ increases with uninformed demand. $\footnotesize M$ decreases with the  information cost $\footnotesize C$.

---

# Tradeoff: security vs market efficiency 
Block time increases security, but also increases variance of types. 
$$ \scriptsize\text{when types are uniform: }
\begin{cases}\scriptsize
\text{participation cutoff } v_M &=
\scriptsize \overline v -  \frac{\overline v}{M-1}\log\left(\frac{\pi+M\,\left(\overline v-\pi\right)}{\overline v}\right) \underset{M\rightarrow\infty}{\longrightarrow} \overline v 
\\ \scriptsize
\text{liquidity } \kappa  &= 
\scriptsize \sqrt{2\,\frac{(M-1)^3 N}{(M-1) M (\pi -\overline v) ((M-1) \pi -(M-3) \overline v)-2\, M \,\overline v^2 \,\log \left(\frac{\overline v}{M (\overline v- \pi)+\pi }\right)}} 
\\ \scriptsize
\text{volumes } \tilde\delta(v_i)&=
\scriptsize \frac{1}{2(M-1)}\left(\left(M \,\left(\overline{v}-\pi\right)+\pi\right)\,e^{-\frac{(M-1) (\overline{v}-v_i)}{\overline{v}}}
-\overline{v}\right)\\ 
\scriptsize
\text{priority fee } \varphi(v_i)&=
\scriptsize \frac{\left(\overline v-\pi\right) \,\left(\overline v\,\left(M-3\right)-\pi\,\left(M-1\right) \right))}{M-1}
-
\frac{2\, \overline v^2}{(M-1)^2}\log \left(\frac{\overline v}{M (\overline v-\pi)+\pi }\right) \\ \scriptsize
\text{number of transactions/active traders: }M\,(1-F\left(\underline v_M\right)) &= 
\scriptsize
 \frac{M}{M-1}\log\left(M-\pi\frac{M-1}{\overline v}\right) 
\end{cases}
$$

![equilibriumUniform](./images/equilibriumUniform.png){style="transform: translate(90%, -8%); width: 350px"}


---
section: Macroeconomics
layout: center
---

**Fayçal Drissi, Zach Feinstein, Basil Williams (2026). Macroeconomics of liquid staking**
<center> 
University of Oxford, Imperial Business School, Stevens Institute of Technology

**Link**:  [faycaldrissi.com/staking_talk](https://www.faycaldrissi.com/staking_talk/)
</center>

---

# Blockchains pay for security with issuance

### Proof of stake

- Lock native token on the blockchain to participate in the consensus protocol
- <u>Economic security</u>: blockchain pays for security with **issuance** (staking rewards)
- Blockchain incentivises good behaviour with **slashing**

<br>
<br>

<v-click>

### Liquid staking

- <u>**Deposit assets**</u>: users lock tokens (ETH, SOL) in a liquid staking protocol
- <u>**Receive the derivative token**</u>: protocol issues a token (stETH) that represents the staked assets
- <u>**Earn rewards**</u>: staking reward increases the value of the derivative token
- <u>**Examples**</u>: Lido, Rocket pool, Ankr, Marinade Finance (Solana)

</v-click>

<!--<v-click>

### Benefits: 
  - No opportunity costs: assets remain accessible for DeFi use
  - Better economic security

</v-click>-->

---

# Fact #1: LSTs enable DeFi
### Users can uses LSTs in DeFi
- Uniswap pools (stETH)
- Aave Interest Bearing STETH  (stETH as collateral to borrow  assets)
<br><br>

<v-click>

### Market cap of LSTs in increasing

![LIDO stETH issuance](./images/LIDOsteth.png){style="transform: translate(-8%, 0%); width: 480px"}
![Rocket Pool LST](./images/RocketPoolLST.png){style="transform: translate(94%, -100%); width: 480px"}

</v-click>

---

# Fact #2: liquid staking dominates solo staking

- Liquid staking is easy
<v-click>

- Liquid staking reduces reward risk
$\implies$ strategic complementarity

<v-click>

- Liquid staking represents the majoritary of staking

![stakinghistory](./images/solostakers.png){style="transform: translate(0%, 0%); width: 900px"}

</v-click>
</v-click>

---

# Motivation
 

<p style="text-align: center;"><h3> <u>Question</u> <br>

What are the effects of liquid staking on the macroeconomics of blockchains ?
</h3>
</p>

<v-click>

<br>
<br>
<br>

<p style="text-align: center;"><h3> <u>Some answers</u> <br>

The tension between staking and DeFi (productivity) is necessary for issuance & slashing to influence user incentives

LSTs eliminate the tension between staking and DeFi
<br>

Natural forces will migrate DeFi from native ETH to LSTs
<br>

Issuing (or slashing) ETH would no longer affect user incentives

</h3>
</p>


</v-click>

---

# Blockchain economy without liquid staking tokens

* Small open economy with continuum of homogeneous users (mass one).
* Consumption good normalized to $1$ USD.

<v-click>

* Blockchain issuance is exogenous 
$$dI_t^e/I_t^e$$

<v-click>

* Blockchain users  maximise expected log utility of consumption 
$$E_0\int_0^{\infty} e^{-\beta\,t}\,\log(c_t)\,dt$$

<v-click>


- Users allocate wealth across:
  1. Consumption (USD)
  2. DeFi  (with native ETH)
  3. Staking


</v-click>
</v-click>
</v-click>


---

# Issuance / slashing in USD

* Price of ETH $P=\$1$. 
* Supply of ETH $Q=2\, \footnotesize\text{ETH}$ 
* Stakers hold $1$ ETH, DeFi users hold $1$ ETH

$\implies$ market cap of ETH = $Q\times P = \$\,2.$
<v-click>

* Protocol issues $1$ ETH to stakers $\implies$ new supply $Q = 3 \, \footnotesize\text{ETH}$ 
<v-click>

* Market Cap in USD does not change $\implies$ price adjusts to $P = \$\,2/3$
<v-click>

$\implies$  stakers hold 2 ETH worth $\$\,4/3$,  DeFi users 1 ETH worth $\$\,2/3$

<v-click>

**$\implies$ Issuance redistributes USD wealth from ETH holders to stakers, it does not create/destroys USD**
$$
\boxed{\text{ETH Issuance policy } dI^e_t/I^e_t \equiv \text{USD tax policy } dI^\$_t/I^\$_t \text{ on DeFi users}}
$$

<br>

<v-click>

### Slashing
* Slashing burns ETH of stakers and transfers value to non‑stakers via price adjustment

</v-click>
</v-click>
</v-click>
</v-click>
</v-click>

---

# Blockchain economy without liquid staking tokens

- $S_t\,$:  USD value of aggregate staked ETH
- $D_t$:  USD value of aggregate productive ETH

<br>

### Dollar return to DeFi: $\small \qquad \qquad \qquad \qquad \qquad \underbrace{\mu^{\$}\,dt+\sigma^{\$}\,dZ_{t}}_{\text{productivity rate}}-\underbrace{\frac{S_{t}}{D_t}\frac{dI_{t}^{\$}}{I_{t}^{\$}}}_{\text{issuance tax}}+\underbrace{\gamma\frac{S_{t}}{D_t+S_t}dN_{t}}_{\text{deflation}}$

<v-click>

### $\footnotesize \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\quad\swarrow\qquad\qquad\qquad \nearrow$

### Dollar return to staking: $\small \qquad \qquad \qquad \qquad \qquad \qquad  \underbrace{\frac{dI_{t}^{\$}}{I_{t}^{\$}}}_{\text{issuance}}-\underbrace{\gamma\frac{D_{t}}{D_t+S_t}dN_{t}}_{\text{slashing}}$

<v-click>

- Users determine their allocation $\theta_D$
$$
dx_t = \theta_{D,t} \times \text{DeFi} + (1-\theta_{D,t}) \times \text{staking } - \text{consumption} 
$$ 

</v-click>
</v-click>

<br>




---

# Blockchain macroeconomics

### Equilibrium and clearing conditions
- Prices clear when ETH demand from users matches ETH supply
$
\qquad \qquad \qquad P_t \, Q_t = S_t + D_t = x_t
$
<v-click>

- Only DeFi (productivity) and consumption create/destroy USD in the economy
$
\quad d(P_t\,Q_t) = D_t (\mu^{\$}\,dt+\sigma^{\$}\,dZ_{t} ) - \beta\, P_t\,Q_t\,dt
$
<v-click>

- ETH supply changes due to issuance/slashing
$
\qquad\qquad\qquad \qquad \qquad\qquad\ \ \ \text{tax policy} ={\color{red} \mu_{\iota}^{\$}}\,dt+{\color{red} \sigma_{\iota}^{\$}}\,dZ_{t}+{\color{red}\gamma_{\iota}^{\$}}\,dN_{t}
$
<v-click>

- Staked / productive ETH determined by user decisions $\qquad\qquad\qquad\qquad\quad\ \ D_t = \theta_D\,P_t\,Q_t \qquad S_t = (1-\theta_D)\,P_t\,Q_t$
<v-click>

<br>

### Solution

$$\footnotesize
\text{allocation } = \theta_D(\gamma,{\color{red} \mu_{\iota}^{\$}}, {\color{red} \sigma_{\iota}^{\$}}, {\color{red}\gamma_{\iota}^{\$}}) \qquad \qquad \qquad \text{ETH prices: } \begin{cases}
\text{drift}  & = \mu_P(\gamma,{\color{red} \mu_{\iota}^{\$}},{\color{red} \sigma_{\iota}^{\$}}, {\color{red}\gamma_{\iota}^{\$}})\\
\\\text{productivity shocks}  & = \sigma_P(\gamma, {\color{red} \mu_{\iota}^{\$}},{\color{red} \sigma_{\iota}^{\$}}, {\color{red}\gamma_{\iota}^{\$}}) \\
\\\text{slashing shocks} & =\gamma_P(\gamma, {\color{red} \mu_{\iota}^{\$}}, {\color{red} \sigma_{\iota}^{\$}}, {\color{red}\gamma_{\iota}^{\$}})
\end{cases}
$$

<!--<v-click>
- <u>**Policy objective**</u>: ETH prices
$$\footnotesize
\begin{cases}
\text{Drift} & =\underbrace{\theta_{D}\,\mu^{\$}}_{\text{productivity}}-\underbrace{\left(1-\theta_{D}\right)\mu_{\iota}^{e}}_{\text{inflation}}-\underbrace{\beta}_\text{consumption}+\underbrace{\left(1-\theta_{D}\right)\sigma_{\iota}^{e}\left(\left(1-\theta_{D}\right)\sigma_{\iota}^{e}-\theta_{D}\,\sigma^{\$}\right)}_{\text{covariance issuance/defi}}\\
\\\text{Productivity shocks}  & =\underbrace{\theta_{D}\,\sigma^{\$}}_{\text{DeFi risk}}-\underbrace{\left(1-\theta_{D}\right)\sigma_{\iota}^{e}}_{\text{issuance}}\\
\\\text{slashing shocks} & =\underbrace{\gamma\,\frac{1-\theta_{D}}{1+\left(1-\theta_{D}\right)\left(\gamma_{\iota}^{e}-\gamma\right)}}_{\text{\text{slashing/deflation}}}-\underbrace{\gamma_{\iota}^{e}\,\frac{1-\theta_{D}}{1+\left(1-\theta_{D}\right)\left(\gamma_{\iota}^{e}-\gamma\right)}}_{\text{\text{issuance}}}
\end{cases}
$$

</v-click> -->

<v-click>

### Policy

* <u>**Policy tools**</u> (slashing, ETH issuance) affect USD wealth of users $\implies$ influence incentives 
* <u>**Policy objectives**</u> can be attained (Kose, Rivera and Saleh (2021), Jermann (2023), Cong, He and Tang (2022), and others)

</v-click>
</v-click>
</v-click>
</v-click>
</v-click>

---
layout: two-cols-header
---

# Blockchain economy with only liquid staking tokens

::left::

<br>
<br>
<br>
<br>

### Users allocate wealth across:
  * Consumption (USD)
  * DeFi <u>**with LSTs**</u>
  * Staking with LSTs

<br>



::right::

<v-click>

### Dollar returns -- <u>only ETH</u> in DeFi

- DeFi: $\qquad \text{productivity rate}-\text{issuance tax}+\text{deflation}$

$$\footnotesize 
\qquad\qquad\qquad\qquad\qquad\swarrow\qquad\qquad\qquad \nearrow 
$$

- Staking: $\qquad\qquad\qquad\quad  \text{issuance}\quad- \quad\text{slashing}$

<br>
<br>
<br>
<br>

<v-click>

### Dollar returns -- <u>only LSTs</u> in DeFi
- Staking: $\qquad\qquad\quad\qquad\qquad\quad$ <u>**zero**</u>
<br>
<br>

- DeFi: $\qquad\qquad\quad\qquad\qquad\underbrace{\mu^{\$}\,dt+\sigma^{\$}\,dZ_{t}}_{\text{productivity rate}}$


</v-click>
</v-click>

---

# Consequences
- **ETH issuance** as reward to staking no longer affects the incentives to staking/DeFi.

<br>

- **Slashing** no longer affects USD wealth $\implies$ no longer affects staker incentives.

<br>

<v-click>

- **Centralisation**: total stake at the hand of liquid staking protocols

<br>

<v-click>

- **Centralisation**:
  * Issuance is a temporary transfer of wealh from stakers in the pool that wins the block, to other stakers
  * Aggregating in one liquid staking pool minimizes wealth variance $\implies$ one surviving pool is the dominant strategy when (symmetric) liquid staking pools compete.


</v-click>
</v-click>


---

# Ethereum today

* Users can be productive with both LSTs and ETH
<br>
<br>

<v-click>

* Users allocate wealth across:
  * Consumption (USD)
  * DeFi (with LSTs)
  * DeFi (with ETH)
  * Staking (with LSTs)

<v-click>
<br>

* <u>**Productivity rates**</u> of both tokens are positively correlated


<v-click>

<br>

- For simplicity: <u>**no slashing**</u>

</v-click>

</v-click>

</v-click>

---

# Dollar returns

- DeFi with LSTs $\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad \underbrace{\mu^{\$}\,dt+{\color{red}\sigma^{\$}\,dZ_{t}}}_{\text{LST productivity rate}}+\text{issuance}$

$$
\qquad\qquad\qquad\qquad\qquad\qquad\qquad\quad\uparrow
$$
- DeFi with native tokens $\qquad\qquad\qquad\qquad\qquad\qquad \underbrace{\mu^{\$}\,dt+{\color{blue}\sigma^{\$}\,dW_{t}}}_{\text{ETH productivity rate}}-\text{issuance tax}$
$$
\qquad\qquad\qquad\qquad\qquad\swarrow
$$
- Staking with LSTs $\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\quad \text{issuance}$

- Correlation: accessibility to DeFi with LSTs
$$
\langle {\color{blue}W},{\color{red}Z}\rangle = \rho > 0
$$



---
layout: two-cols-header
---

# Issuance/correlation favour LSTs

::left::

###  $\qquad$ Issuance
![issuance](./code/issuance_nocost.png){style="transform: translate(0%, 0%); width: 450px"}

::right::

<v-click>

###  $\qquad$ Correlation
![correl](./code/correl_nocost.png){style="transform: translate(0%, 0%); width: 450px"}

</v-click>

---

# Strategic complementarity

- DeFi with LSTs $\qquad\qquad\qquad\qquad\qquad\quad \underbrace{\mu^{\$}\,dt+{\color{red}\sigma^{\$}\,dZ_{t}}}_{\text{LST productivity rate}}-\underbrace{c\left(\text{LST}_t\right) dt}_{\text{endog liq cost stETH}}+\text{issuance}$

$$
\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\quad\uparrow
$$
- DeFi with native tokens $\qquad\qquad\qquad\qquad \underbrace{\mu^{\$}\,dt+{\color{blue}\sigma^{\$}\,dW_{t}}}_{\text{LST productivity rate}}-\underbrace{c\left(D_t\right)dt}_{\text{endog liq cost ETH}}-\text{issuance tax}$
$$
\qquad\qquad\qquad\qquad\qquad\qquad\qquad\swarrow
$$
- Staking with LSTs $\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad \text{issuance}$

---
layout: two-cols-header
---

# Liquidity costs  $c\left(x\right) = a - b\,x$

::left::

###  $\qquad$ Without strategic complementarity
![issuance](./code/issuance_nocost.png){style="transform: translate(0%, 0%); width: 450px"}

::right::

###  $\qquad$ With strategic complementarity
![correl](./code/issuance_cost.png){style="transform: translate(0%, 0%); width: 450px"}

---
layout: two-cols-header
---

# Liquidity costs  $c\left(x\right) = a - b\,x$

::left::

###  $\qquad$ Without strategic complementarity
![issuance](./code/correl_nocost.png){style="transform: translate(0%, 0%); width: 450px"}

::right::

###  $\qquad$ With strategic complementarity
![correl](./code/correl_cost.png){style="transform: translate(0%, 0%); width: 450px"}


---

# Conclusion


- Natural forces will lead to $100\%$ liquid staking $\implies$ issuance is not effective

<v-clicks>

- Is it good or bad ? 
  - <u>**bad**</u>: slashing has no effect, no social planning, centralisation
  - <u>**good**</u>: economic security, productivity

- Demand for native ETH can be controlled with gas fees <br> $\implies$ decreases productivity / adoption

- <u>**Future work**</u>: decentralised staking / distributed validator technology (DVT) <br> $\implies$ competition between blockchain and liquid staking protocols
</v-clicks>

---
section: Asset Pricing
layout: center
---

**Fayçal Drissi, Kose John, Fahad Saleh (2026). Bitcoin as a Hedge Asset**

<center> 
University of Oxford, NYU Stern, University of Florida

**Link**:  [faycaldrissi.com/files/mempools.pdf](https://www.faycaldrissi.com/files/mempools.pdf)
</center>

---




---
layout: end
---

Thank you !

These slides:  [faycaldrissi.com/staking_talk/](https://www.faycaldrissi.com/staking_talk/)
