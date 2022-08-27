# TARN-Swap

A target accumulated redemption note (TARN) is a structured coupon bond that will be compulsively terminated one the accumulated coupon breaches a pre-determined barrier (see https://finpricing.com/lib/EqBarrier.html). If structured coupons in a TARN are functions of some selected index interest rates, the TARN is called interest rate TARN.

In particular, if structured coupons are functions of a single selected index rate, it is called single index interest rate TARN. These functions are usually affine-linear with respect to the index rate and may be capped and floored.

Further, if the slope-coefficient in the affine linear function is negative, it is also called an inverse floater TARN in the market. Popular indices are LIBOR, SOFA, OIS, etc.4

An interest rate TARN swap is a structured swap contract with a regular funding leg and a structured leg. The coupons in the structured leg are defined as the same as in the corresponding interest rate TARN. Moreover, the swap has a mandatory termination once the accumulated structure coupon breaches a pre-determined barrier.

This article only handles the following cases: 1) structured coupons are linked to a single index rate, 2) structured coupons are affine-linear with respect to the index with possible caps and floors, 3) a single currency is applied to both swap legs, and 4) the swap is not callable during its life.

A two-factor Gaussian HJM interest rate term structure model is applied to price an interest rate TARN swap, in which a Monte Carlo simulation approach is used. The interest rate term structure model is calibrated to the swaption market.
An interest rate TARN swap is a special cap-floor swap which will be terminated immediately after the accumulated coupon breaches a target. If we set a target high enough, the swap becomes virtually a regular cap-floor swap. 

In fact, an interest rate TARN swap can be decomposed into a regular cap-floor swap and a so-called target redemption component. The target redemption component can be treated as a separable derivative product to cancel the remaining swap.

Let us first consider structured coupons in the structured leg of the swap without the mandatory termination feature. In this case, it is a cap-floor swap. Let L be the rate index with a given term and consider the following rate defined as

A cap-floor swap is a forward contract to exchange accrual interests between a funding leg and a structured cap-floor leg. For simplicity, there is only one specified funding index rate for the funding leg and with a possible funding spread term profile.

For cap-floor leg, the coupon rates are defined with a single specified term index, i.e., the structured coupon rate is a special case in the definition above. 

Interest rate payments for both legs are uncertain at the beginning of the contract. To avoid trivial cases, we assume that a valuation time t is always prior to fixing times provided specified otherwise. The time-t value of the swap is thus the sum of tine-t values of the two legs.




