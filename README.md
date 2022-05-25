# Credit-Intelligent-Advisor

Hey guys!
This repository contains my Credit-Intelligent-Advisor project that I proposed to our CEO at capital markets, CTBC Bank.


# Introduction
Credit bond market has long been considered illiquid and non-transparent.
Predicting the market performance of individual new issue bond, which has the most liquidity in its life-cycle.
I aim to predict market performance using fundamental & technical data as features to capture opportunities of capital gains. For example, when traders do not have strong view towards specific issuance, model can help them create undiscovered return.

# Dataset

The datasets used in the project (market & individual company data) were directly pulled out from Bloomberg Terminal.
Currently collected data ranges from 2012 to 2021 period.
The model is currently running on Google Colab, in the future I will switch to Bloomberg BQNT Platform.

# Methodology and Results

I use Graph Convolutional Networks(GCN) as the model.
I select “Issuer” and “Industry” to construct the graph, every node is a data point, in COO format, [0, 1] means node 0 has same issuer or industry with node 2.

# Discussion and Conclusion

I got 74.96% train accuracy and 66.28% test accuracy
From Confusion Matrix we can count out F1-score is 0.6456 

# References

[1] https://pytorch-geometric.readthedocs.io/
[2] https://github.com/rusty1s/pytorch_geometric/tree/master/examples
[3] https://peaceful0907.medium.com/
[4] https://www.youtube.com/watch?v=WeHM2xpYQpw

