# Market Risk Back Test Exception

Backtest exceptions occur when Clean P&L and/or Model P&L exceed Model VaR on an absolute basis. The use of both model P&L and clean P&L for exception reporting gives granularity in the drivers of the exception.

The backtest P&L calculations are based on the actual day-over-day changes in market inputs observed. The market inputs must be the same as those used for official valuation thereby establishing a direct linkage to P&L.

Root cause investigations are required to validate instances of backtest exceptions. Investigation documentation should be prepared, including the root cause, the analysis performed to find the root cause, and the follow-up actions to be taken, if any.

Exceptions may be classified as legitimate, or false. For instances where the exceptions are deemed as false, such as spurious market data input, and IT system issues, appropriate operational procedures need to be followed for issue resolution including reruns, market data reloading/recalibration, etc.

Comparison of day-over-day market data change with the changes or scenario shocks implied by the VaR scenario can be utilized to validate the exceptions.

Cases where the market move is the only cause of the exception, no further validations are required. The conclusion can be further proved by a comparison of the market data change with its historical trend, showing that the move is in a greater magnitude than the historical data, as well as what’s captured in the VaR window.

Cases where the market move is in line with its historical trend, implying the VaR scenario shocks are relatively benign, the framework around reviewing Model Assumptions can be applied for further investigations. The Risk Measurement Performance Review has responsibility for this examination.

Root cause of the exceptions under this category can be broadly attributed to:

-       Valuation Approach driven: Clean P&L has risks modelled through a full revaluation approach but DGV VAR uses a sensitivity based approach.
-       Risk Factor Selection driven: greek approximation, market data proxies, etc.

Management must formally document all backtesting exceptions and the specific reason(s) for each tolerance level breach must be quantified and explained. Further, management is required to maintain documentation that assesses the cause of backtesting exceptions and identifies any action undertaken as a result of the exception. Finally, management must track all backtesting exceptions, not just “official” breaches used in determining the regulatory multiplier.

Root cause should be clearly documented, with supporting analysis memo attached if necessary. Reference should be made to PAA data, realized market movement that drove the BT breach, risk exposures, and VaR risk factor data.

Over time, the backtest results should be summarized as the number of exceptions over rolling periods (monthly, quarterly, annually) to provide an ongoing validation of the accuracy of the VaR model. The Risk Measurement and Performance Review Stream will regularly review the exception count as a validation for the model. In the Fundamental Review of the Trading Book, Basel provides some guidelines as to the expected number of breaches for an accurate model (see https://finpricing.com/lib/FiBondCoupon.html)
