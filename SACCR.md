SA-CCR Questions

**Q1. Why alpha is 1.4?**

$$EAD\  = \ alpha\ *\ (RC + PFE)$$

Answer:

In contrast to loan exposures, derivative exposures are uncertain. Thus,
a EPE (Effective Positive Exposure) for a derivative is bound to
understate portfolio capital as compared to the certain LEE (loan
equivalent exposure) for loan exposures[^1].

Alpha is used to convert Expected Effective Positive Exposure (EEPE)
into a (LEE)[^2]. The value of 1.4 is carried over from the alpha value
set by the Basel committee for the internal model method (IMM)[^3] in
2005. This calibration is based on studies dating back to 2003 viz^2^.

a)  Canabarro, E, E Picoult and T Wilde (2003): "Analysing counterparty
    risk", Risk, September, pp 117--22.

b)  Wilde, T (2005): "Analytic methods for portfolio counterparty risk"
    in M Pykhtin (ed), Counterparty credit risk modelling, Risk Books.

c)  [ISDA-TBMA-LIBA (2003): Counterparty risk treatment of OTC
    derivatives and securities financing
    transactions.](https://www.sec.gov/rules/proposed/s72103/isda020404a.pdf)

Initially, Evan Picoult, (MD, Head of Risk Method & Analytics, Risk
Architecture, Citigroup, New York in 2002) wrote a proposal to an ISDA
working group that recommended we define a quantity called "alpha," a
scaling factor to transform the EPE into a good loan equivalent[^4].

Alpha is defined as the ratio of two quantities A/B, where^4^:

-   A = The EC (Economic Capital) for counterparty risk measured with
    full simulation

-   B = The EC for counterparty risk measured assuming a constant
    exposure profile for each counterparty equal to its EPE.

The full simulation is as follows^4^:

a)  Simulate thousands of paths of changes in market factors over time.

b)  For each simulated path of the market, calculate the potential
    exposure to each counterparty at many future dates.

c)  For each simulated path of the market, calculate potential loss by
    simulating counterparty defaults, at many future dates.

d)  Repeat the simulation of potential defaults and recoveries for each
    stimulated path of market rates.

e)  Calculate the final loss distribution by appropriately aggregating
    the potential loss distribution for each simulated path of the
    market.

f)  Economic capital from a default-only perspective would then be
    derived from the loss distribution by measuring its UL at the
    appropriate confidence level.

Subsequently, Canabarro, Picoult and Wilde (2003) used a one-factor
credit risk portfolio model to study the sensitivity of α to various
model inputs and parameters under the assumption of wrong-way risk.
Their base case resulted in α = 1.09. After adding wrong-way risk to the
same model, Wilde (2005) obtained for the same base case α = 1.21.
ISDALIBA-TBMA (2004) reports estimates of α in the range 1.07-1.10
calculated by four banks using their internal models for their own
portfolios.

**Under the IMM, α is fixed at a rather conservative level of 1.4 in
2005.**

**Q2: Why is there a 2\*(1-Floor) in the denominator of the multiplier
formula?**

$$\mathbf{multilpier\  = \ min\ }\left\{ \mathbf{1\ ;\ Foor\  + \ (1 - Floor}\mathbf{)*}\mathbf{*exp}\left( \frac{\mathbf{V - C}}{\mathbf{2*(1 - Floor)*}\mathbf{\text{AddOn}}^{\mathbf{\text{aggregate}}}} \right) \right\}$$

Answer:

The SA-CCR specifies the PFE as the product of the aggregate (i.e.
netting-set-level) add-on and a multiplier W (.)[^5].

$$PFE = W\ \left( \frac{V - C_{\text{CE}}}{\text{AddOn}^{\text{aggregate}}} \right)*\text{AddOn}^{\text{aggregate}}\ $$

A netting-set level add-on is an estimate of the netting set PFE under
the four assumptions viz:

a)  The current MTM value of each trade is zero (i.e., trade is
    at-the-money, ATM).

b)  The bank neither holds nor has posted collateral for the netting
    set.

c)  There are no cash flows within the capital horizon of one year.

d)  The evolution process for MTM value of each trade follows arithmetic
    Brownian motion with zero drift and fixed volatility.

These assumptions are needed to obtain the linear dependence of the
aggregate add-on on a\
single dynamic quantity -- the volatility of the netting set MTM value.
The most important benefit of this dependence is that one can aggregate
add-ons from a trade level to a netting-set level as if they were
standard deviations. Furthermore, the SA-CCR calibration can be reduced
to making assumptions on volatilities and correlations of market risk
factors that drive trade MTM values^5^.

The multiplier is derived under the conditions when the first two
assumptions (a & b above) are relaxed and the impact of current MTM and
collateral is factored in.

Further, as per the assumption (d) above, the netting set future MTM
value is normally distributed. However, MTM values of real netting sets
are likely to exhibit heavier tail behaviour than the one of the normal
distribution. To account for this possibility, a more conservative
multiplier function (Exponential) was chosen[^6]:

$$W_{\exp}(y)\  = \ min\ \left\{ 1,\ exp\ (\frac{y}{2}) \right\}$$

Where the factor of 2 appears in the denominator in order the match the
slope of $W_{\text{model}}(y)\ at\ y\  = 0$ ;
$y\  = \ \left\lbrack V\  - \ C_{\text{CE}} \right\rbrack\ /\ AddOn$ ;

While the exponential multiplier is significantly more conservative than
the model-based multiplier, concerns were raised that the multiplier
would still approach zero with infinite overcollateralisation. To
address this concern, a floor *F* was added to the exponential
multiplier in a manner that preserves the function slope at the origin.

The solid curve in Figure below this function with *F* = 5% currently
chosen in the SA-CCR.

$$W_{SA - CCR}\ (y)\  = \ min\ \left\{ 1,\ F\  + \ (1 - F)\ exp\ \left( \frac{y}{2(1 - F)} \right) \right\}$$

![](media/image1.png){width="5.373611111111111in"
height="4.347916666666666in"}

**Q3. Why is there 1.4 and 0.6 in the Effective Notional Formula?**

$$\mathbf{\text{Effective\ Notional}}_{\mathbf{j}}^{\mathbf{(IR)}}\mathbf{\  = \ }\sqrt{\left( \mathbf{D}_{\mathbf{j}\mathbf{1}}^{\mathbf{(IR)}} \right)^{\mathbf{2}}\mathbf{\  + \ }\left( \mathbf{D}_{\mathbf{j}\mathbf{2}}^{\mathbf{(IR)}} \right)^{\mathbf{2}}\mathbf{\  + \ }\left( \mathbf{D}_{\mathbf{j}\mathbf{3}}^{\mathbf{(IR)}} \right)^{\mathbf{2}}\mathbf{\  + \ 1.4*}\mathbf{D}_{\mathbf{j}\mathbf{1}}^{\mathbf{(IR)}}\mathbf{*}\mathbf{D}_{\mathbf{j}\mathbf{2}}^{\mathbf{(IR)}}\mathbf{\  + \ 1.4*}\mathbf{D}_{\mathbf{j}\mathbf{2}}^{\mathbf{(IR)}}\mathbf{*}\mathbf{D}_{\mathbf{j}\mathbf{3}}^{\mathbf{(IR)}}\mathbf{\  + \ 0.6*}\mathbf{D}_{\mathbf{j}\mathbf{1}}^{\mathbf{(IR)}}\mathbf{*}\mathbf{D}_{\mathbf{j}\mathbf{3}}^{\mathbf{(IR)}}}$$

Answer:

Correlations between the maturity buckets are set as follows[^7]:
$\text{\ \ }\rho_{12}\  = \ \rho_{23}\  = \ 70\%\ ;\ \ \rho_{13}\  = \ 30\%$\
Historical correlations between swap rates of different tenors has been
used as proxies for correlations between MTM values of trades with
different remaining maturities.

Historical correlations between weekly changes of swap rates of
different tenors (between one year and 30 years) for each of four major
currencies (USD, EUR, GBP and JPY) were calculated for the time period
from January 1, 2005 to December 31, 2009[^8].

Such estimation resulted in the following correlation values: 68%
between buckets 1 and 2; 68% between buckets 2 and 3; and 28% between
buckets 1 and 3. These numbers have been then rounded to 70% and 30%.

Hence, 2\*0.7 = 1.4 and 2\*0.3 = 0.6 in the effective notional formula.

**Q4. Why Supervisory Duration formula is as such?**

$$\mathbf{\text{SD}}_{\mathbf{i}}\mathbf{\  = \ }\frac{\mathbf{exp( - 0.05\ *\ }\mathbf{S}_{\mathbf{i}}\mathbf{)\  - \ exp\ ( - 0.05*}\mathbf{E}_{\mathbf{i}}\mathbf{)}}{\mathbf{0.05}}$$

Answer:

A fixed-for-floating IR swap as the most common example of an IR
derivative. Suppose that swap *I* payments start at time *S~i~*, end at
time *E~i~* and refer to notional *N~i~*(t) at time *t*. In the
continuous limit,\
swap MTM value can be written as^7^:

$$V_{i}^{\text{swap}}\ (t)\  = \ \left\lbrack \text{SR}_{i}(t)\  - \ \text{FR}_{i} \right\rbrack\ \int_{\text{max\ }\left\{ S_{i},\ t \right\}}^{E_{i}}{N_{i}\left( \tau \right)\text{\ DF\ }\left( t,\tau \right)\text{dτ}}$$

where SR~i~ (t) is the swap rate at time *t* , FR is the fixed rate and
DF(t ,τ) is the discount factor from time τ to time *t* . The SA-CCR
assumes that all variability of the swap MTM value results from changes
of the swap rate, thus "freezing" the discount factor in the integral.
The IR supervisory factor is meant to capture the one-year volatility of
the swap rate, while the adjusted notional is meant to represent the
value of the integral at time *t* = 0. The SA-CCR approximates the
integral by setting the adjusted notional equal to:

$$d_{i}^{\text{IR}}\  = \ \overline{N_{i}}*\text{SD}_{i}$$

Where, $\overline{N_{i}}$ is the average of the swap notional over the
remaining life of the swap payments and SD~i~ is the supervisory
duration given by

$$\text{SD}_{i}\  = \ \int_{S_{i}}^{E_{i}}{exp\ ( - rt)\ dt}\ \  = \ \frac{\exp\left( - rS_{i} \right)\  - \ exp\left( - rE_{i} \right)\ }{r}$$

With the interest rare set to r = 0.05

**Q5. Why there is a factor of 1.5 in Maturity Factor?**

$$\mathbf{\text{MF}}_{\mathbf{i}}^{\mathbf{(margined)}}\mathbf{\  = \ }\frac{\mathbf{3}}{\mathbf{2}}\sqrt{\frac{\mathbf{\text{MPOR}}}{\mathbf{1\ year}}}$$

Answer:

Maturity factor is used to scale down the volatility of the trade MTM
from one year to the trade remaining maturity *M~i~* (in case of
unmargined transactions) for the trades with *M~i~ \< 1 year*[^9]~.~

$$\text{MF}_{i}^{no - margin}\  = \ \sqrt{\frac{\text{min\ }\left\{ M_{i},\ 1\ year \right\}}{1\ year}}$$

For margined netting sets, the SA-CCR add-on is defined as the expected
increase of the netting set MTM over the MPR^9^. Thus, the maturity
factor in case of margined transactions scales down the time period for
the volatility to the MPOR.

However, the reason scaling of Maturity Factor by 1.5 for margined
transactions is not clear. 1.5 multiplier maintained by Basel in order
to approach the EE of a margined transactions to the one of an
un-margined transaction for MPOR is resulting in double accounting for
the shock (1.5 × 1.4)[^10].

[^1]: Page 6: [Measuring Counterparty Credit Risk for Trading Products
    under Basel II, Bank of
    America](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=941551)

[^2]: Page 5: [Foundations of the standardised approach for measuring
    counterparty credit risk exposures
    (Basel)](https://www.bis.org/publ/bcbs_wp26.pdf)

[^3]: Page 15: [Moody Analytics Introduction to
    SA-CCR](https://www.pwc.com/gx/en/advisory-services/basel-iv/basel-iv-calculating-ead-according-to-the-new-standardizes-approach-for-counterparty-credit-risk-sa-ccr.pdf)

[^4]: Page 7: [Economic Capital for Counterparty Credit Risk by Evan
    Picoult](https://cms.rmau.org/uploadedFiles/Credit_Risk/Library/RMA_Journal/Loan_Loss_Reserves/Economic%20Capital%20for%20Counterparty%20Credit%20Risk.pdf)

[^5]: Page 7: [Foundations of the standardised approach for measuring
    counterparty credit risk exposures
    (Basel)](https://www.bis.org/publ/bcbs_wp26.pdf)

[^6]: Page 16: [Foundations of the standardised approach for measuring
    counterparty credit risk exposures
    (Basel)](https://www.bis.org/publ/bcbs_wp26.pdf)

[^7]: Page 12: [Foundations of the standardised approach for measuring
    counterparty credit risk exposures
    (Basel)](https://www.bis.org/publ/bcbs_wp26.pdf)

[^8]: Page 18: [Foundations of the standardised approach for measuring
    counterparty credit risk exposures
    (Basel)](https://www.bis.org/publ/bcbs_wp26.pdf)

[^9]: Page 9: [Foundations of the standardised approach for measuring
    counterparty credit risk exposures
    (Basel)](https://www.bis.org/publ/bcbs_wp26.pdf)

[^10]: Page 6-7: [Sayah, M. (2017) Counterparty Credit Risk in OTC
    Deriva-tives under Basel III. Journal of Mathemat-ical Finance, 7,
    1-38](https://file.scirp.org/pdf/JMF_2016123016343974.pdf)
