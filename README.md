# Amortizing Bond and Accreting Bond Valuation

An amortizing bond is a bond whose principal (face value) decreases due to repaying part of the principal along with the coupon payments. Each payment to the amortizing bond holder consists of a portion of interest and a portion of principal. While an accreting bond is a bond whose principal increases during the life of the deal. Each payment to the accreting bond holder is just a part of interest. The other part of coupon is added to the principal of the bond. 
An amortizing bond is used specifically for tax purposes as the amortized principal is treated as part of a company’s interest expense. An accreting bond is used to improve the profit of the existing bond and make it more marketable. Pension funds and insurance companies are major investors in accreting bonds.  This presentation gives an overview of amortizing bonds and accreting bonds. 

	Amortizing Bond an Accreting Bond Introduction
	A bond is a debt instrument in which an investor loans money to the issuer for a defined period of time. 
	An amortizing bond is a bond whose principal (face value) decreases due to repaying part of the principal along with the coupon payments.
	Each payment to the amortizing bond holder consists of a portion of interest and a portion of principal.
	An accreting bond is a bond whose principal increases during the life of the deal.
	Each payment to the accreting bond holder is just part of interest. The other part of coupon is added to the principal of the bond.

	The Use of Amortizing Bonds and Accreting Bonds
	An amortizing bond is used specifically for tax purposes as the amortized principal is treated as part of a company’s interest expense.
	The issuer credits the amortized principal amount to interest payable, i.e., an accrued liability.
	An accreting bond is used to improve the profit of the existing bond and make it more marketable.
	Pension funds and insurance companies are major investors in accreting bonds.


	Valuation
	The analytics are similar to a fixed rate bond except the principal amount used for each period may be different. 
	The present value of an amortizing bond or accreting bond is given by
V(t)=∑_(i=1)^n▒〖cP_i e^(-(r_i+s) T_i )+P_n e^(-(r^n+s) T_n ) 〗
where
	t – valuation date
i – ith cash flow from 1 to n
	r_i – continuous compounded interest rate for period (t,T_i)
T_i – coupon payment date of the ith  cash flow
s – credit spread
P – principal amount or face value
c - coupon rate

	Practical Guide
	The present value of a bond computed by any pricing models is the dirty price of the bond. To purchase a bond, the buyer pays this dirty price.
	Although investors pay dirty prices, bonds are typically quoted in terms of clean prices. 
Dirty Price = Clean Price + Accrued Interest
	The Yield-To-Maturity Model is a good tool to compute the present value or the fair value of a bond. But it is very difficult to calculate risk, such as term structure sensitivities, that is more important than the fair value in trading, hedging and risk management. Therefore, we introduce the Credit Spread Model for computing both risk and fair value.
	Intuitively,   e^(-(r+s)T)   can be regarded as a credit risk adjusted discount factor.
	To use the model, one should first calibrate the model price to the market quoted price by solving the credit spread. Comparing to curve construction or calibration for exotic products, the solving here is very simple.
	After making the model price equal to the market price, one can calculate sensitivities by shocking interest rate curve and credit spread.
	We use LIBOR curve plus credit spread rather than bond specific curves for discounting because bond specific curves rarely exist in the market, especially issued by small entities. Using LIBOR curve plus credit spread not only accounts for credit/issuer risk but also solves the missing data issue.

 
	A Real World Example

Bond Definition	Principal Schedules
Name	Value	Principal	Start Date
Buy Sell	Buy	100	8/24/2009
Calendar	TOR	98.75	5/31/2010
Coupon Type	Fixed	97.5	11/30/2010
Currency	CAD	95	5/31/2011
First Coupon Date	11/30/2009	92.5	11/30/2011
Interest Accrual Date	8/24/2009	90	5/31/2012
Issue Date	8/24/2009	87.5	11/30/2012
Last Coupon Date	5/31/2019	79	5/31/2013
Maturity Date	11/30/2019	70.5	11/30/2013
Settlement Lag	3	62	5/31/2014
Principal	100	53.5	11/30/2014
Pay Receive	Receive	45	5/31/2015
Day Count	dcAct365	36.5	11/30/2015
Payment Frequency	6M	28.75	5/31/2016
Coupon	0.0434	21	11/30/2016

References:

https://finpricing.com/lib/EqRangeAccrual.html

https://bitbucket.org/cmrm11/fiamortizingbond/downloads/FiAmortizingBond-9.pdf

