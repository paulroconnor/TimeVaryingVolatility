# Time-Varying Volatility Models

## Time-Varying, Stochastic Volatility in Continuous Time
In the Heston model, for example, the constant parameter $\sigma$ is replaced by an Itô process that obeys:

$$
d\sigma^2 = \lambda(\bar{\sigma}^2 - \sigma^2) dt + c \sigma^2 dB
$$

where $\lambda$, $c$, and $\bar{\sigma}^2$ are constants.

## Time-Varying, Stochastic Volatility in Discrete Time
In the GARCH(1,1) model, for example, the constant parameter $\sigma$ is replaced by a time series process of the form:

$$
\sigma^2_t = \kappa(\bar{\sigma}^2 - \sigma^2_{t-1}) + \alpha \sigma^2_{t-1}(z_{t-1}^2 - 1)
$$

where $\alpha$, $\kappa$, and $\bar{\sigma}^2$ are constants.

## Deterministic Volatility
The constant parameter $\sigma$ is replaced by a deterministic function of time $\sigma(t)$, and the variance is replaced by the more general "quadratic variation," given by:

$$
\frac{1}{T} \int_0^T \sigma^2(t) dt
$$


## Geometric Brownian Motion (GBM)
In each case, the stock follows instantaneous geometric Brownian motion of the form:

$$
\frac{dS}{S} = \mu dt + \sigma(t) dB
$$

where $\mu$ is a positive constant for the drift and $\sigma(t)$ is a function of time. This means that over short intervals, the stock follows GBM, but the volatility changes from one interval to the next.
