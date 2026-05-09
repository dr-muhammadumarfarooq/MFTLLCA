# MFTLLCA
Accelerating Life Cycle Inventory Development through Correlation-Aware Multi-Fidelity Transfer Learning: Case Studies in Cradle-to-Gate Manufacturing Energy Modeling

Details can be requested via email: muf@umich.edu

ItemImplementation DetailInput scalingInputs normalized to $[0, 1]$Target scalingAbsolute-maximum scalingANN architectureInput layer, one hidden layer, output layerHidden neurons tested$H \in \{4, 8, 12\}$Learning rates tested$\{0.001, 0.01, 0.1\}$$\lambda$ values tested$\{0.1, 0.3, 0.5, 0.7, 1.0\}$OptimizerAdamSelection metricMinimum validation RMSE; validation $R^2$ as secondary check$\lambda$ during boostingFixed after grid searchAdaptive variableSample-weight distributionBoosting update errorPointwise scaled squared residualMaximum boosting rounds30Stopping criterionLoss below $1 \times 10^{-6}$ or max epoch/boosting limitRolling selected setup$\lambda = 0.5$, 12 hidden neurons, learning rate = 0.01Material-extrusion setup$\lambda = 0.1$, 12 hidden neurons, learning rate = 0.01Evaluation metrics$R^2$, RMSE, MAE, MedAE
