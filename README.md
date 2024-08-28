# contingent_premium_option

A Contingent Premium Option is a type of exotic option where the premium is only paid if the option finishes in-the-money (ITM) at expiration. This differs from standard options where the premium is paid upfront regardless of the option's outcome. The main appeal of contingent premium options is that they provide potential exposure to the underlying asset's movements without an upfront cost, reducing initial outlay.


Underlying Asset (S): The asset on which the option is based (e.g., a stock, index).
Strike Price (K): The price at which the option can be exercised.
Premium (P): The amount that is paid by the holder if the option ends up ITM. The premium is contingent upon the option's final value.
Maturity (T): The time until the option expires.

Call Option: Gives the holder the right to buy the underlying asset at the strike price.
Put Option: Gives the holder the right to sell the underlying asset at the strike price.


The payoff of a contingent premium option depends on whether the option is ITM at maturity.

Call Option Payoff:
1) If the option is ITM, the payoff at maturity T is:
Payoff_call = max(S_T - K, 0) - P
Where:
S_T is the price of the underlying asset at maturity.
K is the strike price.
P is the contingent premium.
2) If the option is out-of-the-money (OTM) at maturity (i.e., S_T <= K), the payoff is:
Payoff_call = 0


Put Option Payoff:
1) If the option is ITM, the payoff at maturity T is:
Payoff_put = max(K - S_T, 0) - P
2) If the option is OTM at maturity (i.e., S_T >= K), the payoff is:
Payoff_put = 0

