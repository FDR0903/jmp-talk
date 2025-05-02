---
layout: cover
class: text-center
title: JMP
theme: academic
titleTemplate: '%s'
favicon: ./images/defiicon.png
author: Fayçal Drissi
themeConfig:
  paginationX: disabled
  paginationY: disabled
  paginationPagesDisabled: [1]
fonts:
  local: Montserrat, Roboto Mono, Roboto Slab # local fonts are used for legal reasons for deployment to https://slidev-theme-academic.alexeble.de and only set up for the example project, remove this line for your project to automatically have fonts imported from Google

mdc: true
---

## Decentralised Finance 

<br>

**Fayçal Drissi**

<br>

Slides: [faycaldrissi.com/jmp-talk](https://www.faycaldrissi.com/jmp-talk)

<br>

[scholar](https://scholar.google.com/citations?user=njvyriQAAAAJ&hl=fr), 
[website](https://www.faycaldrissi.com/), [github](https://github.com/FDR0903)

---

# Decentralised Finance (DeFi)
####  Blockchain technology
* Distributed ledger without central authority
* **Social benefits**: transparency, fewer monopolies, easy value transfer, help underbanked people

<br>


<Footnotes separator>
<Footnote :number=1>
<a href="https://www.banqueducanada.ca/2020/02/note-analytique-personnel-2020-4/">CBDC and Monetary Policy</a>
</Footnote>
<Footnote :number=2>
<a href="https://finance.ec.europa.eu/digital-finance/digital-euro_en/">Digital Euro by the ECB</a>
</Footnote>
<Footnote :number=3>
Cross-border settlement in CBDCs as priority policy of the G20<br> 
<a href="https://www.bis.org/about/bisih/topics/cbdc/rialto.htm">Project Rialto</a>
, <a href="https://www.bis.org/about/bisih/topics/suptech_regtech/pyxtrial.htm">Regulation of asset-backed stablecoins</a>
<br>
<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5080183&dgcid=ejournal_htmlemail_cryptocurrency%3Aresearch%3Aejournal_abstractlink">International Monetary Fund (IMF) On Cross-Border Crypto Flows</a>
</Footnote>
<Footnote :number=4>
<a href="https://www.bis.org/about/bisih/topics/cbdc/mariana.htm">Project Mariana</a>
</Footnote>
<Footnote :number=5>
By Bank of International Settlements, Bank of France, Monetary Authority of Singapore, Central Bank of Malaysia, and Swiss National Bank
</Footnote>
</Footnotes>


---

# Decentralised Finance (DeFi)
####  Blockchain technology
* Distributed ledger without central authority
* **Social benefits**: transparency, fewer monopolies, easy value transfer, help underbanked people <br>
 <br>

#### Applications of blockchains
* Central Bank Digital Currencies (CBDCs) & Tokenization of digital assets <br>
**Economic benefits**: better monetary policy oversight reduced transaction costs<sup>1, 2</sup>
* Inter-bank and cross-border Forex trading: **inter-bank FX Settlement** using **DeFi**<sup>3, 4, 5</sup>
* Decentralised Autonomous Organizations and E-governments
<!--financial (bonds, stocks, ETFs) & non-financial assets (commodities, real estate)<br> **Economic benefits**: reduce transaction costs and processing time-->

<Footnotes separator>
<Footnote :number=1>
<a href="https://www.banqueducanada.ca/2020/02/note-analytique-personnel-2020-4/">CBDC and Monetary Policy</a>
</Footnote>
<Footnote :number=2>
<a href="https://finance.ec.europa.eu/digital-finance/digital-euro_en/">Digital Euro by the ECB</a>
</Footnote>
<Footnote :number=3>
Cross-border settlement in CBDCs as priority policy of the G20<br> 
<a href="https://www.bis.org/about/bisih/topics/cbdc/rialto.htm">Project Rialto</a>
, <a href="https://www.bis.org/about/bisih/topics/suptech_regtech/pyxtrial.htm">Regulation of asset-backed stablecoins</a>
<br>
<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5080183&dgcid=ejournal_htmlemail_cryptocurrency%3Aresearch%3Aejournal_abstractlink">International Monetary Fund (IMF) On Cross-Border Crypto Flows</a>
</Footnote>
<Footnote :number=4>
<a href="https://www.bis.org/about/bisih/topics/cbdc/mariana.htm">Project Mariana</a>
</Footnote>
<Footnote :number=5>
By Bank of International Settlements, Bank of France, Monetary Authority of Singapore, Central Bank of Malaysia, and Swiss National Bank
</Footnote>
</Footnotes>

---
layout: center
---

<p style="text-align: center;"><h2>
It is <b>key</b> to study these new markets to influence policy and practice at early stages, and to achieve its potential <a name="defi1"></a></h2>
</p>

---

# Research agenda

### Blockchain market microstructure and design
* Mathematical tools to describe optimal trading and liquidity provision
* Detect and address design inefficiencies
* Analyse equilibrium properties of price and liquidity in blockchain-based trading systems

<br>

### Monetary policy in decentralised economies

* Macro-finance models to study inflation, adoption, and issuance policies in blockchains
* Examine the impact of the structure of the ecosystem on asset pricing and economic outcomes

<br>

### Blockchain protocol and mechanism design

* Develop improved architectures for automated market makers (AMMs)
* Design market mechanisms for competition over block space allocation


---

# Outline
### Part I: Blockchain market microstructure
* Introduction to Blockchains and Automated Market Makers (AMMs)
* How DEXs constrain strategic behaviour of liquidity providers
* Market design solutions to improve efficiency
 <br><br>
### Part II: Ongoing work
* Monetary policy in blockchain economies (Macro-Finance)
* Bitcoin Asset Pricing
* Designing competition mechanisms for block inclusion
* Market fragmentation in blockchains

---
layout: center
---

<p style="text-align: center;">
<h2>Part I: Decentralised Market Microstructure </h2>
</p>

--- 

# Decentralised Finance: two parts
<br />

### Blockchains

* Infrastructure
* Lifecycle of transactions

<br />
<br />

### Smart contracts

* Public programs on the blockchain: define the rules of interactions
* Immutable and permissionless

<br />
<br />

---

<p style="text-align: center;">
<h2> Decentralised Finance </h2>

<br />

<h3>An ecosystem of smart contracts that <em>mimic</em> traditional financial services without intermediaries <a name="defi1"></a></h3>
</p>

<br />
<br />
<br />

---

<p style="text-align: center;">
<h2> Decentralised Finance </h2>

<br />

<h3>An ecosystem of smart contracts that <em>mimic</em> traditional financial services without intermediaries <a name="defi1"></a></h3>
</p>

<br />
<br />
<br />

<p style="text-align: center;">
<h2> Decentralised exchanges </h2>
<br>
<h3>
Trading platforms where the rules of interaction are encoded in a smart contract operating on the blockchain   <a name="defi2"></a></h3>
</p>

---

# Automated Market Makers

* A liquidity pool for securities $X$ and $Y$
* Available *reserves* $x$ and $y$

![pool1](./images/pool1.png){style="transform: translate(165%, 20%); width: 200px"}

---

# Automated Market Makers

### Two types of participants

* **Liquidity takers (LTs)** trade with the pool

![pool2](./images/pool2.png){style="transform: translate(30%, 50%); width: 500px"}

---

# Automated Market Makers
### Two types of participants
* **Liquidity providers (LPs)** *deposit* assets in the pool or *withdraw* assets from the pool

![pool3](./images/pool3.png){style="transform: translate(31.5%, 51%); width: 500px"}

---

# Automated Market Makers
### Economic principle: bonding curves

*  Iso-liquidity curve or indifference curve (points of same level of liquidity)
$$
\qquad
$$

![BC1](./images/BondingCurves1.png){style="transform: translate(18%, 10%); width: 630px"}

---

# Automated Market Makers
### Liquidity takers

* To buy a quantity $\Delta y$, one pays
$$
\frac{\Delta x}{\Delta y} = \frac{\Phi(y-\Delta y) - \Phi(y)}{\Delta y}
$$

![bc2](./images/bc2.png){style="transform: translate(18%, 10%); width: 630px"}

---

# Automated Market Makers
### Liquidity takers

* To sell a quantity $\Delta y$, one receives
$$
\frac{\Delta x}{\Delta y} = \frac{\Phi(y) - \Phi(y+\Delta y)}{\Delta y}
$$

![bc3](./images/bc3.png){style="transform: translate(18%, 10%); width: 630px"}

---

# Automated Market Makers
### Liquidity takers
* Let $\{x, y\} = \{\Phi(y), y\}$ be the state of the pool.
* **Marginal Price** and **slippage**
$$
\underbrace{\frac{\Phi(y)-\Phi(y+\Delta y)}{\Delta y}
    }_{\text{Price to sell }\Delta y}  \xrightarrow{\Delta y \longrightarrow 0} \underbrace{Z=-\Phi'(y) }_{\text{marginal price}}\xleftarrow{0\longleftarrow \Delta y} \underbrace{\frac{\Phi(y-\Delta y)-\Phi(y)}{\Delta y}}_{\text{Price to buy }\Delta y}
$$


---

# Automated Market Makers
### Liquidity takers
* Let $\{x, y\} = \{\Phi(y), y\}$ be the state of the pool.
* **Marginal Price** and **slippage**
$$
\underbrace{\frac{\Phi(y)-\Phi(y+\Delta y)}{\Delta y}
    }_{\text{Price to sell }\Delta y}  \xrightarrow{\Delta y \longrightarrow 0} \underbrace{Z=-\Phi'(y) }_{\text{marginal price}}\xleftarrow{0\longleftarrow \Delta y} \underbrace{\frac{\Phi(y-\Delta y)-\Phi(y)}{\Delta y}}_{\text{Price to buy }\Delta y}
$$
* **Price impact**
$$
-\Phi'(y+\Delta y)
    \xleftarrow{\text{after a sell}}  \underbrace{Z=-\Phi'(y) }_{\text{marginal price}}\xrightarrow{\text{after a buy}} -\Phi'(y-\Delta y)
$$


---

# Automated Market Makers
### Liquidity takers
* Let $\{x, y\} = \{\Phi(y), y\}$ be the state of the pool.
* **Marginal Price** and **slippage**
$$
\underbrace{\frac{\Phi(y)-\Phi(y+\Delta y)}{\Delta y}
    }_{\text{Price to sell }\Delta y}  \xrightarrow{\Delta y \longrightarrow 0} \underbrace{Z=-\Phi'(y) }_{\text{marginal price}}\xleftarrow{0\longleftarrow \Delta y} \underbrace{\frac{\Phi(y-\Delta y)-\Phi(y)}{\Delta y}}_{\text{Price to buy }\Delta y}
$$
* **Price impact**
$$
-\Phi'(y+\Delta y)
    \xleftarrow{\text{after a sell}}  \underbrace{Z=-\Phi'(y) }_{\text{marginal price}}\xrightarrow{\text{after a buy}} -\Phi'(y-\Delta y)
$$
* Approximations
$$
\begin{cases}
\text{slippage} & \approx \frac12 \Phi''(y) \Delta y\\
\text{impact} & \approx  \Phi''(y) \Delta y
\end{cases}
$$

---

# Automated Market Makers
### Liquidity takers
![cvxty](./images/convexity1(1).png){style="transform: translate(30%, 0%); width: 600px"}
<font size ="1">
Scatter plots of the execution cost and the price impact of 2.622 million LT transactions against approximations. The transactions  are between January 2023 and December 2023 in 38 different Uniswap v3 pools.
</font>

<!--

# Automated Market Makers
### Liquidity takers


* **Price impact** following a buy order of volume $\Delta y$
$$
Z_0 = -\Phi'(y) \longrightarrow Z_1 = -\Phi'(y-\Delta y) \approx Z_0 + \Phi''(y)\,\Delta y
$$
* **Price impact** following a sell order of volume $\Delta y$
$$
Z_0 = -\Phi'(y) \longrightarrow Z_1 = -\Phi'(y+\Delta y) \approx Z_0 - \Phi''(y)\,\Delta y
$$-->

---

# Automated Market Makers
### Liquidity takers

- Optimal liquidation strategies in DEXs<sup>1, 2</sup>

$$
\begin{cases}
d\tilde{Z}_{t} & =dZ_{t}-c_{t}\,\nu_{t}\,dt\\
dy_{t} & =-\nu_{t}\,dt\\
d{x}_{t} & =\left(\tilde{Z}_{t}-\frac{1}{2}\,c_{t}\,\nu_{t}\right)\,\nu_{t}\,dt\\
\sup_{\nu} & \mathbb E_{t,x,y,Z,S}\left[x_{T}^{\nu}+y_{T}^{\nu}\,\tilde{Z}_{T}-\alpha\,\left(y_{T}^{\nu}\right)^{2}-\phi\,\int_{t}^{T}\left(y_{s}^{\nu}\right)^{2}\,ds\right]
\end{cases}
$$

- Approximation method for semilinear PDEs
- Backtest on real data

<Footnotes separator>
<Footnote :number=1>
Cartea, Álvaro, Fayçal Drissi, and Marcello Monga. "Decentralised finance and automated market making: Execution and speculation." <b>2nd round JEDC</b>
</Footnote>
<Footnote :number=2>
Cartea, Álvaro, Fayçal Drissi, and Marcello Monga. "Execution and statistical arbitrage with signals in multiple automated market makers." <b>2023 IEEE</b></Footnote>
</Footnotes>


---

# Automated Market Makers
### Liquidity providers
* Liquidity providers deposit/withdraw liquidity <!--without changing the marginal price $Z$-->


---

# Automated Market Makers
### Liquidity providers
* Liquidity providers deposit/withdraw liquidity
* They earn proportional fees

---

# Automated Market Makers
### Liquidity providers
* Liquidity providers deposit/withdraw liquidity
* They earn proportional fees
* They incur adverse-selection costs<sup>1</sup>
<!--* Change in wealth of LPs against not providing liquidity-->
$$
0 \ge \underbrace{\Phi(y-\Delta y)-\Phi(y)}_{\text{cash received}}+\underbrace{\Delta y \, \Phi'(y-\Delta y)}_{\text{change in value}} \approx -\frac12 \Phi''(y) \, \Delta y^2
$$
<!--$$
\text{L}_{t}= -\frac{1}{2}\int_{0}^{t}\,\Phi''\left(y_{s}\right)\,d<y,y>_{s}
$$-->
<br><br><br>

<Footnotes separator>
<Footnote :number=1>
<a href="https://www.tandfonline.com/doi/full/10.1080/1350486X.2023.2277957">Cartea, Á., Drissi, F., & Monga, M. (2023). Predictable losses of liquidity provision in constant function markets and concentrated liquidity markets.<br><b> Applied Mathematical Finance</b></a>
</Footnote>
</Footnotes>

---

# Losses in Ethereum and Uniswap<sup>1</sup>

| | Average      | Standard Deviation | 
|  :---  | :---        |    :----:   | 
| Losses  | $-1.64\%$ | $7.5\%$ |
| Revenue |  $0.155\%$   | $0.274\%$        |
| Hold time |   $6.1$ days   |  $22.4$ days       |
<!--| Number of transactions per LP | $11.5$ | $40.2$ | -->



<Footnotes separator>
<Footnote :number=1>
<a href="https://epubs.siam.org/doi/full/10.1137/23M1602103">Cartea, Á., Drissi F., & Monga M. (2024) Decentralised Finance and Automated Market Making: Predictable Loss and Optimal Liquidity Provision.<br><b>SIAM Journal on Financial Mathematics</b></a>
</Footnote>
</Footnotes>

---

# Losses in Ethereum and Uniswap

* LPs can reduce these losses significantly<sup>1</sup>
$$
\sup_{\nu}\mathbb{E}\bigg[\underbrace{\left(Y_{T}+Q_{T}^{\nu}\right)\,S_{T}^{\nu}}_{\text{replication}}-\underbrace{\int_{0}^{T}\left(S_{t}^{\nu}+k\,\nu_{t}\right)\,\nu_{t}\,dt}_{\text{replication cost}}-\underbrace{\tfrac{1}{2}\phi\int_{0}^{T}\left(Q_{t}^{\nu}+Y_{t}\right)^{2}\,dt}_{\text{inventory aversion}}\bigg]
$$
where
$$
\begin{cases}
Y_{T} & =\text{DEX position}\\
S^{\nu} & =F+\text{impact}\\
F_t & =F_{0}+\int_{0}^{t}A_{u}\,du+\sigma\,W_{t}\,,\\
A & =\text{general latent trading signal}
\end{cases}
$$
* Characterise solution as that of an FBSDE
* Reduce the FBSDE to a Lotka-Volterra system
* Backtests

<Footnotes separator>
<Footnote :number=1>
<a href="https://www.tandfonline.com/doi/full/10.1080/1350486X.2023.2277957">Drissi, F., Jaimungal, S., Wu, X. Hedging of liquidity positions un Automated Market Makers</a>
</Footnote>
</Footnotes>


---

# Losses in Ethereum and Uniswap

* The core issue persists: LPs have limited strategic flexibility
* **Solution**: design DEXs that give LPs the tools to express strategic preferences

---
layout: center
---

<p style="text-align: center;"><h1>
Improving AMMs <a name="design"></a></h1>
</p>
<br>

Cartea, Drissi, Sánchez-Betancourt, Siska, Szpruch (2024)

Strategic bonding curves in automated market makers

<!--

# Why AMMs

* Price to add a transaction to the blockchain: **gas fee**
    * Gas fees scale with transaction complexity
    * Significantly expensive to run traditional markets on a blockchain
* **Constraints**: computational simplicity
* **Solution**: Automated market makers (AMMs)-->

---

# AMM design

### Objective
* Provide strategic tools to LPs
<br><br>

### Constraints
* Use  **available information** on the blockchain
* **Simple mechanics** to update prices and reserves

<Footnotes separator>
<Footnote :number=1>
<a href="https://www.tandfonline.com/doi/full/10.1080/1350486X.2023.2277957">
</a>
</Footnote>
</Footnotes>

---

# AMM design

### Decentralised Liquidity Pool (DLP)

* Reserves $\{x, y\}$

* Marginal Price $Z$

* LTs impact the price according to impact functions $\{\eta^b, \eta^a\}$

* The slippage is determined by quote functions $\{\delta^b, \delta^a\}$<sup>1</sup>

<br><br><br><br><br><br>

<Footnotes separator>
<Footnote :number=1>
We derive conditions for the impact and quote functions to prevent roundtrip arbitrage and price manipulation 
</Footnote>
</Footnotes>

---

# AMM design

### Liquidity takers 

* $\left(N_t^b\right)_{t\in[0,T]}$ and $\left(N_t^a\right)_{t\in[0,T]}$: counting processes for the number of sell and buy orders of minimum trading volume $\zeta$

* The dynamics of the DLP reserves
$$
d y_{t}=\,\zeta\, d N_{t}^{b}-\zeta\, d N_{t}^{a}
$$
$$
d x_{t}=\,-\zeta\,\left( Z_{t^-}-\delta_{t}^{b} \right)\,d N_{t}^{b}
+
\zeta\,\Big(Z_{t^-}+\delta_{t}^{a}\Big)\, d N_{t}^{a}
$$

* The dynamics of the marginal price
$$
d Z_{t}=-\eta^b(y_{t^-})\,d N_{t}^{b} + \eta^a(y_{t^-})\,d N_{t}^{a}
$$

<!--### Liquidity providers
* They set the functions $\{\eta^b,\eta^a,\delta^b,\delta^a\}$ periodically-->

--- 

# AMM design

### AMM $\subset$ DLP

* Let $\Phi$ be the trading function of an AMM
* Let the impact functions of the DLP be
$$
\eta^a(y) = \Phi'(y)  - \Phi'(y-\zeta)\,\quad\text{and}\quad  \eta^b(y) = -\Phi'(y) + \Phi'(y +\zeta)
$$
* Let the quote functions of the DLP be
$$\delta^a_t = \frac{\Phi(y_{t^-} - \zeta) - \Phi(y_{t^-})}{\zeta} + \Phi'(y_{t^-}) + \pi \, \zeta
$$

$$
\delta^b_t = \frac{\Phi(y_{t^-} + \zeta) - \Phi(y_{t^-})}{\zeta} - \Phi'(y_{t^-}) + \pi \, \zeta
$$
* Then DLP $\equiv$ AMM !

--- 

# AMM design

### Strategic tools of LPs
* LPs can set these functions according to strategic preferences
* **Restrictions**: employ information on the blockchain
* **Objective**: filter the fundamental price from the order flow in the blockchain and adapt the price of liquidity

---

# Strategic bonding curve

### A model
* Let $P$ be the (unobserved) fundamental price
* We discretize $Z - P$ into $M$ values, or regimes.
* $g \notin \mathbb F$ is a CTMC with finite state space $\mathcal S = \{1, \dots, M\}$ that describes the regimes. 
* The transition rate matrix is $\Pi$
<!--    * Regime $1$ corresponds to $P<<Z$
    * Regime $M$ corresponds to $Z<<P$-->

---

# Strategic bonding curve
### A model
* LTs are sensitive to the **fundamental price**. The vectors 
$$\boldsymbol{c}^b = \{c^{b,1},\dots,c^{b,M}\} \quad \text{and} \quad \boldsymbol{c}^a = \{c^{a,1},\dots,c^{a,M}\}$$ 
describe the **baseline  intensity** of the trading flow at the bid/ask in each regime $j\in\{1,\dots,M\}$
* LTs are sensitive to the **slippage**. If $g_t = j$
$$
\lambda^{b,j}_t(\delta^b_t)=  c^{b,j}\,e^{-\kappa\,\delta_{t}^{b}} 
$$
$$
\lambda^{a,j}_t(\delta^a_t)= c^{a,j}\,e^{-\kappa\,\delta_{t}^{a}}
$$

---

# Strategic bonding curve
### Filtering from the trading flow
* The DLP does not  observe the regime $g$.
* We can assign a probability $\Psi^{j}_{t}$ to be in regime $j$ at time $t$ given $\mathcal{F}_t$ 
$$
 \Psi^{j}_{t} = \mathbb{E}\left[ \mathrm{1}_{g_t = j} \,\mid\,\mathcal{F}_t\right]
$$

--- 

# Strategic bonding curve
### Filtering from the trading flow
* The  filter $\Psi^{j}_{t}$ satisfies 

$$
\Psi^{j}_{t} = \frac{\Gamma^j_t}{\sum_{i=1}^M\Gamma^i_t} \,,
$$
where the process $\Gamma^j$, for $j\in\{1,\dots,M\}$, follows the dynamics
$$
\frac{d \Gamma^j_t }{\Gamma^j_t} = \left( \lambda^{a,j}_{t^-}\left(\delta_t^a\right) - 1\right)\left(d N^{a}_t -d t\right) +  \left( \lambda^{b,j}_{t^-}\left(\delta_t^b\right) - 1\right)\left(d N^{b}_t -d t\right) + \frac{\sum_{i=1}^{M}\Gamma_{t^{-}}^{i}}{\Gamma_{t^{-}}^{j}} \,\pi_{ji}\,d t
$$

---

# Strategic bonding curve


### Adaptive control problem
* We compute the optimal quote functions $\{\delta^b, \delta^a\}$ for fixed impact functions $\{\eta^b,\eta^a\}$

---

# Strategic bonding curve

### Adaptive control problem
* We compute the optimal quote functions $\{\delta^b, \delta^a\}$ for fixed impact functions $\{\eta^b,\eta^a\}$
* We consider Poisson processes $N^b$ and $N^a$ with projected stochastic intensities $\hat{\lambda}^{b}$ and $\hat{\lambda}^{a}$
$$
\begin{cases}
\hat{\lambda}_{t}^{b} =  e^{-\kappa\,\delta_{t}^{b}}\, \mathrm{c}^{b}\cdot\mathrm{\Psi}_{t} \\
\hat{\lambda}_{t}^{a} =  e^{-\kappa\,\delta_{t}^{a}}\, \mathrm{c}^{a}\cdot\mathrm{\Psi}_{t}
\end{cases}
$$

---


# Strategic bonding curve

### Adaptive control problem
* We compute the optimal quote functions $\{\delta^b, \delta^a\}$ for fixed impact functions $\{\eta^b,\eta^a\}$
* We consider Poisson processes $N^b$ and $N^a$ with projected stochastic intensities $\hat{\lambda}^{b}$ and $\hat{\lambda}^{a}$
$$
\begin{cases}
\hat{\lambda}_{t}^{b} =  e^{-\kappa\,\delta_{t}^{b}}\, \mathrm{c}^{b}\cdot\mathrm{\Psi}_{t} \\
\hat{\lambda}_{t}^{a} =  e^{-\kappa\,\delta_{t}^{a}}\, \mathrm{c}^{a}\cdot\mathrm{\Psi}_{t}
\end{cases}
$$
* The performance criterion[^pcm] (well-posed)
$$
\mathbb{E}_{t,x,y,z,\mathrm{\Psi}}\left[x_{T}+y_T\,Z_T\right]
$$

<br><br>

[^pcm]: The set of admissible bonding curves is
$
\mathcal A_t~=~\Big\{ (\delta^b_s, \delta^a_s)_{s \in [t,T]},\ \mathbb R^2\text{-valued},\ \mathbb F\text{-adapted, square-integrable, bounded from below}\Big\}
$

---

# Strategic bonding curve
### The solution
* The optimal bonding curve (in feedback form)
$$
\delta_{t}^{\star,b}=\frac{1}{\kappa}-\frac{\theta\left(t,y+\zeta,\frac{\tilde{\mathrm{\psi}}\odot\tilde{\mathrm{c}}^{b}}{\psi\cdot\mathrm{c}^{b}}\right)-\theta\left(t,y,\tilde{\mathrm{\psi}}\right)}{\zeta}+\frac{1}{\zeta}\left(\frac{\tilde{\mathrm{\psi}}\odot\tilde{\mathrm{c}}^{b}}{\psi\cdot\mathrm{c}^{b}}\cdot\nabla_{\tilde{\mathrm{\psi}}}\theta-{\tilde{\mathrm{\psi}}}\cdot\nabla_{\tilde{\mathrm{\psi}}}v+\left(y+\zeta\right)\eta^{b}(y)\right)
$$
$$
\delta_{t}^{\star,a}=\frac{1}{\kappa}-\frac{\theta\left(t,y-\zeta,\frac{\tilde{\mathrm{\psi}}\odot\tilde{\mathrm{c}}^{a}}{\psi\cdot\mathrm{c}^{a}}\right)-\theta\left(t,y,\tilde{\mathrm{\psi}}\right)}{\zeta}+\frac{1}{\zeta}\left(\frac{\tilde{\mathrm{\psi}}\odot\tilde{\mathrm{c}}^{a}}{\psi\cdot\mathrm{c}^{a}}\cdot\nabla_{\tilde{\mathrm{\psi}}}\theta-{\tilde{\mathrm{\psi}}}\cdot\nabla_{\tilde{\mathrm{\psi}}}v-\left(y-\zeta\right)\eta^{a}(y)\right)\,.
$$

---

# Strategic bonding curve
### Experiments
* Two regimes: $c^b = 5\times c^a$ and $c^a = 5 \times c^b$ 

![bc11](./images/oracle_bonding_curve_1-1.png){style="transform: translate(55%, 10%); width: 400px"}

<!--::right::
![bc12](./images/oracle_bonding_curve_2-1.png){style="transform: translate(0%, 10%); width: 400px"}-->

---
layout: two-cols-header
---

# Strategic bonding curve
### Experiments
* Scenario I : $100\%$ arbitrageurs
* Scenario II: $50\%$ arbitrageurs, $50\%$ noise traders

::left::
| | Average$^1$      | Standard Deviation | 
|  :---  | :---        |    :----:   | 
| DLP (Sc. I) | $-0.04\%$ | $0.719\%$ | 
| DLP (Sc. II)   | $0.717%$ | $2.584\%$ |
| Buy and Hold |  $0.01\%$   | $0.741\%$        |
| Uniswap$^2$ |   $-1.485\%$    |  $7.812\%$ |

1. $30$-minutes performance of LPs 
2. Using $42,022$ LP operations between 5 May 2021 and 30 April 2022*

::right::

![experiments1](./images/DLPexperiments.png){style="transform: translate(10%, 0%); width: 400px"}


---
layout: center
---

<p style="text-align: center;"><h1>
Blockchain protocols and market microstructure <a name="bd"></a></h1>
<br><br><br>

Capponi A., Cartea A., Drissi, F. (2025)

Price Formation and Equilibrium Liquidity in Blockchains

</p>



---

# Blockchain protocol
The blockchain protocol determines the lifecycle of transactions and adds new cost structures

---

# Blockchain protocol
The blockchain protocol determines the lifecycle of transactions and adds new cost structures

* Transactions sent continuously and stored in memory pools (**pre-trade transparency** and **PGAs**) 
<br><br><br>

![blockchain1](./images/blockchaincreation1.png){style="transform: translate(20%, 0%); width: 680px"}

---

# Blockchain protocol
The blockchain protocol determines the lifecycle of transactions and adds new cost structures

* Transactions sent continuously and stored in memory pools (**pre-trade transparency** and **PGAs**) 
* At the end of an Epoch, with length **block time**, a validator is chosen
<br><br>

![blockchain1](./images/blockchaincreation2.png){style="transform: translate(20%, 3%); width: 680px"}

<!---

#  Decentralised Exchanges

* Liquidity supply and price of liquidity
* Price dynamics-->

---

# Blockchain protocol
The blockchain protocol determines the lifecycle of transactions and adds new cost structures

* Transactions sent continuously and stored in memory pools (**pre-trade transparency** and **PGAs**) 
* At the end of an Epoch, with length **block time**, a validator is chosen
* The validator creates a new block with transactions from the memory pool

![blockchain1](./images/blockchaincreation3.png){style="transform: translate(20%, 0%); width: 680px"}

---

# Blockchain protocol

* **Priority fee**: incentivise validators to prioritise a transaction in the block

![mempools](./images/mempools.jpeg){style="transform: translate(25%, 0%); width: 580px"}

---

# Contribution

- We present a three stage model to describe the economic consequences of priority fees and block time on **liquidity**, **price discovery**, and **market frictions**

---

# Contribution
- We model strategic interactions between takers and suppliers of liquidity as a three-stage game
    - **stage 0**: multiple traders decide whether to acquire information
    <br><br>
    Informed traders enter only if expected gains exceed a fixed cost
![model1](./images/model1.png){style="transform: translate(10%, 0%); width: 700px"}

---

# Contribution
- We model strategic interactions between takers and suppliers of liquidity as a three-stage game
    - **stage 0**: multiple traders decide whether to acquire information
    - **stage 1**: liquidity suppliers set the AMM’s reserves<br>
    The optimally balance adverse selection losses against profits from uninformed demand
![model1](./images/model2.png){style="transform: translate(10%, 0%); width: 700px"}

---

# Contribution
- We model strategic interactions between takers and suppliers of liquidity as a three-stage game
    - **stage 0**: multiple traders decide whether to acquire information
    - **stage 1**: liquidity suppliers set the AMM’s reserves
    - **stage 2**: informed traders compete with priority fees (English auction ending with FPSB auction)
![model1](./images/model3.png){style="transform: translate(10%, -10%); width: 700px"}

---

# Contribution
- We model strategic interactions between takers and suppliers of liquidity as a three-stage game
    - **stage 0**: multiple traders decide whether to acquire information
    - **stage 1**: liquidity suppliers set the AMM’s reserves
    - **stage 2**: informed traders compete with priority fees
![model1](./images/model4.png){style="transform: translate(10%, 0%); width: 700px"}


---

# Results

- **Block time**, combined with **priority fees**, enhances DEX efficiency:
    - **Price efficiency**: more informed traders enter as block time increases
    - **Market liquidity**: competition stabilises informed volume, reduces adverse selection, and improves liquidity
- Slow information dissemination
    - Informed traders reveal signals only right before block creation
- When informed traders are limited (due to high barriers or low adoption):
    - Beyond a threshold block time, liquidity suppliers withdraw and markets shut down

---
layout: center
---

# Future of decentralised finance

---

# DeFi protocols

| **Service**       | **DeFi**      | **TradFi** | 
|  :---         | :---        |    :----   | 
| Trading |  DEXes (Uniswap, Curve)|  Brokers & exchanges | 
| Credit | Lenders post assets in liquidity pools, and borrowers borrow against collateral (Compound, Aave) |  Commercial banks| 
| Payments |  Transfer of value onchain via DeFi protocols (Flexa, Sablier Finance) |  Cash, Credit/debit cards, accounts | 
| Insurance |  Customers buy tokens in exchange for cover against digital or real-life risks (Armor, Nexus Mutual) |  Insurance firms | 
| Investment and Derivatives | Funds are allocated to pools based on preset risk tolerance. Vehicles include crypto-indices, derivatives, options, and perpetual futures (Yearn Finance, dY dX) | Investment funds | 

---
layout: center
---

<p style="text-align: center;">
<h2>Part II: Ongoing work </h2>
</p>

---

### Decentralised Monetary Policy
### Drissi F., Feinstein, Z., \& Williams, B.

* Continuous-time macro-finance model of crypto exchange rates and blockchain monetary policy
* Layer-2 blockchains increase exchange rate volatility and reduce decentralisation
* Dollar economy shocks help blockchain ecosystems in the short run but hurt in the long run

---

### An Economic Model of Bitcoin as a Hedge
### Drissi F., John, K., Saleh, F. 

* Explains why Bitcoin is perceived as a hedge against traditional markets
* Asset pricing model: government adjusts monetary policy to crypto, agents shift wealth based on heterogeneous beliefs
* In equilibrium:
    * Misbeliefs self-fulfil, driving decorrelation during crises
    * Bitcoin transaction demand creates correlation in normal times

---

### Block Space Competition Design
### Cartea A., Drissi, F., Lillo, F., Palmari G.

* Study the design of priority gas auctions in blockchains
* Propose contests (not auctions) as a new mechanism for block priority competition
    * In contests, higher bids raise winning chances but do not guarantee priority
* When participation is endogenous, contests increase trading volume and liquidity, while preserving validator revenue

---

### Public and Private Order Flow in Blockchains
### Cartea A., Drissi, F., Garcia-Arenas, G. 

* Study how order flow splits between public and private endpoints in blockchains
* Public endpoints expose transactions to MEV extraction by bots
* Private endpoints offer privacy but delay or uncertainty in block inclusion
* Characterising equilibrium segmentation is key to understanding blockchain microstructure

---
layout: end
---

[faycaldrissi.com/jmp-talk](https://www.faycaldrissi.com/jmp-talk)
