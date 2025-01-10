# <font color=#e92063>The International Effects of the Fed's UMP</font>

Hi! This page is still in development. Thanks for your patience!

## <font color=#e92063>Introduction</font>

This is a friendly (updated) version of my undergraduate thesis. In this project, I estimate a traditional VAR with exogenous variables to investigate the international effects of the implementation of unconventional monerary policy tools on the Mexican Economy, namely the *Forward Guidance* and the *Quantitative Easing*. You can see the python code in this [Jupyter Notebook](WuXia.html).

## <font color=#e92063>What does Unconvetional Monetary Policy mean?</font>

First, we need to state what the Federal Reserve (the Fed) is, why it is important and then how it relates to the Monetary Policy. Well, with the risk of oversimplifying, the Fed is in charge of two things: reaching maximum employment and keeping stable prices (low inflation). This is also known as "dual mandate." The set of tools that the Fed can use to reach its objectives is calles the Monetary Policy.

Now, if there's an Unconventional Monetary Policy, that implies that there's also a **Conventional** Monetary Policy. The "Conventional" Monetary Policy is the set of tools that the Federal Reserve **usually** applies to reach its goals. That's basically the short term interest rate. The Fed buys and sells short term government bonds to influence its prices and therefore their interest rate. When the short term interest rate moves, it generates a chain reaction in the financial system that spreads through several channels and into the real economy.

### **The Monetary Policy at the Zero Lower Bound**

What happens when the interest rate is really close to zero? This situation was believed to be the limit of the monetary policy tools to influence the economy. When the interest rate reached the zero lower bound (ZLB) during the Great Financial Crisis, the unconventional monetary policy (UMP) made its appearance.

This new tool (at least for the Fed) allowed the Federal Reserve to buy not only short term bonds, but also long term bonds and virtually any asset class. So it wouldn't influence only the short term interest rate, but also longer parts of the interest rate curve. This received the name of "Quantitative Easing" a.k.a. throwing money from helicopters (figuratively). In addition, the announcements made by the Fed contained information about the future monetary policy decisions with the objective of manipulating the market expectations about the future interest rates. This one is called "Forward Guidance."

Those are the two main tools of Unconventional Monetary Policy.

## <font color=#e92063>How can we measure these effects?</font>

When investigating this policies, the researchers stumbled upon the problem of measuring the stance of the monetary policy since the short term interest rate was pretty much fixed at the ZLB, but they knew the Federal Reserve was aggressively expanding their monetary policy. Some used the long term interest rate, some used the size of the balance sheet of the Fed, and so on it goes the list. There isn't still a consensus about which metric to use, but the Wu-Xia shadow short rate seems to be a promising alternative.

In simple terms, the Wu-Xia shadow short rate tries to estimate the value that the short term interest rate would have in the abscence of the zero lower bound. In theory, it's build to capture also the effects of the market expectations, so we should be able to measure both, the quantitative easing and the forward guidance. In this exercise, this is the variable we will use to measure the monetary policy stance.

## <font color=#e92063>Data</font>

To analyze this dynamic, we need to model the relevant relationships inside the domestic economy. At the same time, we need to incorporate the effect of external variables, including our US monetary policy measure: the Wu-Xia shadow short rate. At the end of this page, I'll leave the sources and series ID of the data I'm using. All variables are included as monthly observations.

To describe the macroeconomic dynamic of the Mexican economy, we will choose indicators of the domestic income, prices, monetary policy and exchange rate. For the external variables, we'll incorporate relevant indicators of the US economy. In addition, we need to include in indicator of market volatility to try and filter the effects of risk on the domestic variables.

### **Endogenous Variables**

We're using data from the INEGI for the Mexican economy, with the exception of short term the interest rate that we get from the Mexican Central Bank (Banxico). The domestic income will be measured by the General Index of Economic Activity (IGAE), the price level by the General Consumption Price National Index (INPC), for the exchange rate, we'll use the USD/MXN FIX exchange rate, and for the monetary policy we're using the weighted median Equilibrium Interbank Interest Rate (TIIE). The INPC, IGAE, and exchange rate are included as Year-on-Year logarithmic growth rates.

{!international_ump_effects/elements/UMP_VAR_Endogenous.html!} 

### **Exogenous Variables**

The data for the US economy is available at the St. Louis Federal Reserve Economic Data website. The foreign income is measured by the US Industrial Production Index (INDPRO), the financial risk by the Volatility Index (VIX), and the monetary policy stance by the Wu-Xia shadow short rate. In this case, only the INDPRO is transformed to be included as logarithmic Year-on-Year growth rate. In the graphic below, the Effective Federal Funds Rate is shown as reference to compare the shadow short rate.

{!international_ump_effects/elements/UMP_VAR_Exogenous.html!} 

## <font color=#e92063>Empirical Estimation</font>

### Frequentist Model

Placeholder...

### Bayesian Model

Placeholder...

## <font color=#e92063>Results</font>

Placeholder...

## <font color=#e92063>Conclusions</font>

Placeholder...

## **Appendix**

### Model testing

Placeholder...

### Structural Breaks

Placeholder...

</br></br></br></br>