# WPM Statistical Models

**A framework for data-driven prediction and retrodiction.**

This repository collects papers on the WPM framework and its statistical and mathematical foundations. Prediction estimates future values, events, distributions, fields, or regions from observed histories. Retrodiction uses later observations to infer earlier states, events, or complete candidate histories while preserving uncertainty and alternative explanations.

WPM organizes these tasks around a declared target, a requested horizon, and alternative representations of the available data. Historical extent (`W`) and internal resolution (`m`) define forecasting lenses. Their performance forms a target-specific resolution landscape, whose connected low-risk regions are called **pockets**. Pocket geometry, signed responses, and temporal histories support representation selection, forecast combination, and compatible transfer between systems.

The default forecasting and retrodiction models learn from permitted observations and available outcomes; they are not supplied the system's true governing equation or hidden states. Physical equations in the papers explain examples, constraints, and separately declared model variants. The collection connects the foundational n/s scaling-spectrum study to the general WPM architecture, mathematical methods, and applications in AI training, quantum systems, weather, and historical reconstruction.

## Core papers in the root folder

The root papers introduce the scaling representation and general architecture, then develop landscape construction, pocket operations, transfer, predictive optimization, and inverse recovery.

### [An n/s Scaling-Spectrum Framework for Generalized Moment Scaling](NS_Equations.pdf)

Introduces a conditional scaling-spectrum model with separate coordinates for curvature, baseline scaling, and signed-moment asymmetry. Synthetic and reference-data studies test parameter recovery and applicability; prospective prediction of unseen moment orders helps identify where the model works and where it fails.

### [A Unified Framework for Multiscale, Spatial, and Cross-Domain Prediction](A_Unified_Framework_for_Multiscale_Spatial_and_Cross_Domain_Prediction.pdf)

Presents the general WPM architecture: normalize system coordinates and target meaning, construct target-conditioned resolution landscapes, retain useful pockets, and select Fixed, Multi, or Auto forecasting policies. It covers scalar, probabilistic, field, and region-valued predictions, together with failure diagnosis and adaptation.

### [Pocket Arithmetic and Interaction in WPM](01_Pocket_Arithmetic_and_Interaction.pdf)

Develops operations on signed response packets and represented fields, including superposition, Gaussian kernels, overlap, and fitted relational operators. It distinguishes a geometric pocket from a field component or physical source, and tracks alignment, dependence, identifiability, and approximation error.

### [Resolution Landscapes in WPM](02_Landscape_Construction_and_Dynamics.pdf)

Explains how to build causal risk landscapes from forecasts issued at historical cutoffs and outcomes that have become available. It develops pocket extraction, geometry, coordinate metrics, stability bounds, and temporal identity, showing why accurate risk values do not automatically preserve basin structure.

### [Cross-Family and Partial-Family Prediction in WPM](Cross_Family_and_Partial_Family.pdf)

Formulates transfer through separate checks on coordinates, target semantics, and forecasting eligibility. It distinguishes averaging alternative forecasts from assembling required components, supports selective transfer and abstention, and states the assumptions needed for risk transport and shared latent-coordinate recovery.

### [Optimization for Prediction in WPM](Optimization_for_Prediction.pdf)

Develops target-specific lens selection and forecast aggregation using error dependence, regularization, and delayed feedback. It also covers predictive distributions, conditional uncertainty guarantees, and cost-sensitive decisions while keeping the requested forecast horizon fixed.

### [Source and Relational Equation Recovery with WPM](Source_and_Relational_Equation_Recovery.pdf)

Treats hidden-source and equation recovery as inverse problems defined by the observation map and admissible model class. Worked cases cover anchors, third-source inversion, nonlinear branches, changing or delayed interactions, and missing histories, with rank conditions separating recoverable quantities from unresolved alternatives.

## Application folders

- [AI System](AI%20System/): Papers on data-driven prediction of AI-training progress, structural transitions, oscillation, instability, plateaus, failure, and optimization response.
- [Quantum Systems](Quantum%20Systems/): Papers on observation-based quantum-system forecasting and compatible cross-family or partial-family transfer.
- [Weather Forecasting](Weather%20Forecasting/): Papers on transferring weather predictors across locations and regimes using aligned observations, targets, and compatibility checks.
- [Historical Past Events](Historical%20Past%20Events/): Papers on data-driven retrodiction of past states and events using alternative-history maps, uncertainty-aware smoothing, and causal memory.

## Reading the collection

Start with the unified framework for the overall architecture and the n/s paper for its scaling-spectrum research foundation. The landscape and pocket-arithmetic papers develop the mathematical objects; transfer, optimization, and recovery extend their use. The application folders then specialize those methods to particular observations and targets.

The revised methods papers primarily provide conditional derivations, worked examples, and application procedures. Constructed examples and any cited empirical findings should be read according to their stated assumptions, target definitions, and evidence scope.
