# Talks

Talks are 20 minutes long, including 5 minutes allocated for questions from the audience.	

## Early-morning Section

**Chair:** Chris Rackauckas

{{anchor intro}}
* **Introduction and State of SciML**

    *Time:* 9:00AM - 9:30AM

    *Speaker:* Chris Rackauckas

{{anchor climacore}}
* **SciML for Climate: Integrating ClimaCore.jl with OrdinaryDiffEq**

    *Time:* 9:30AM - 9:50AM

    *Speaker:* Dennis Yatunin 

    *Abstract:* [ClimaCore.jl](https://github.com/CliMA/ClimaCore.jl) is a toolkit for spatially discretizing PDEs into systems of ODEs, with a particular emphasis on the needs of Earth system models (ESMs). Due to the skewed aspect ratio and the effects of gravity and Earth's rotation in such models, the resulting systems of ODEs tend to be very stiff in the vertical direction, requiring the use of implicit-explicit (IMEX) solvers. This talk will describe our efforts to implement and integrate our work with the SciML ecosystem.

{{anchor pumas}}
* **Understanding heterogeneous health outcomes with SciML and Pumas**

    *Time:* 9:50AM - 10:10AM

    *Speaker:*  Niklas Korsbo

    *Abstract:* What is driving disease progression, what effect does a drug have, and why do different patients have different outcomes? At [Pumas-AI](https://pumas.ai), we are mixing SciML with statistical and dynamical modelling to predict and optimise patient outcomes. Here, we explore the ideas of SciML within healthcare and demonstrate how it can be used to not only help develop dynamical models of disease progression and drug effect but also to predict variations in outcomes based on patient information.

{{anchor hydrology}}
* **Neural ODEs in Hydrology**

    *Time:* 10:10AM - 10:30AM

    *Speaker:* Marvin Höge

    *Abstract:* For stream flow predictions in hydrology commonly two types of models are used: deep learning models (high predictive performance) and ODE-based conceptual hydrologic models (fully interpretable, encoding scientific assumptions). We introduce hydrologic Neural ODE models that fuse both approaches and have all benefits: We obtain state-of the-art predictive performance and gain insights into the dynamics of model processes and states. We demonstrate the approach on a large real-world data set.

{{anchor derivatives}}
    
* **Computing derivatives for chaotic and hybrid systems**

    *Time:* 10:30AM - 10:50AM

    *Speaker:* Frank Schafer

    *Abstract:* In this talk, we present shadowing methods for chaotic dynamical systems and continuous-adjoint sensitivity methods for hybrid differential equations modeling explicit and implicit events. The methods are implemented in the DiffEqSensitivity package. Possible fields of application for these tools range from model discovery with explicit dosing times in pharmacology, over accurate gradient estimates for chaotic fluid dynamics, to the control of open quantum systems.

## Late-morning Section

**Chair:** Samual Isaacson

{{anchor keynote}}
* **Keynote:** Simulating stochastic dynamical systems with Runge-Kutta type schemes

    *Time:* 11:00AM - 11:40AM

    *Speaker:* Andreas Rößler

    *Abstract:* Parts of the presentation are joint work with Claudine von Hallern (Universität Hamburg), Felix Kastner (Universität zu Lübeck)
   and Jan Mrongowius. 
   
   In many mathematical models differential equations are used to 
describe the fundamental dynamical system. In order to capture uncertainty
in such models often stochastic differential equations (SDEs) are applied.
We consider the problem of numerical simulations for SDEs.
Therefore, we discuss the concept of stochastic Runge-Kutta methods
that turned out to allow for efficient higher order approximation methods
converging to the solution in the root mean square sense. Special emphasis
is given on the simulation of the Levy area that is essential for higher
order approximations. A new algorithm for the approximation of Levy areas
is presented that is available as a Julia software toolbox. 
Finally, we give a brief outlook to the simulation
of stochastic partial differential equations (SPDEs). Here, some recent 
results on derivative-free Milstein type approximation schemes are 
presented.
     
   *About:* Dr. Andreas Rößler is a professor of mathematics at the Institute of Mathematics at Universität zu Lübeck. His research interests include numerical methods for stochastic ordinary differential equations (SODEs), stochastic partial differential equations (SPDEs), stochastic differential algebraic equations (SDAEs), and stochastic Runge-Kutta methods.

{{anchor mtkinternals}}
* **Internals of ModelingToolkit**

    *Time:* 11:40AM - 12:00PM

    *Speaker:* Yingbo Ma

    *Abstract:* Diving into acausal modeling and internal algorithms of [ModelingToolkit.jl](https://github.com/SciML/ModelingToolkit.jl). In this talk, we will cover various structural simplification algorithms used in ModelingToolkit.jl and the future development goals of ModelingToolkit.

    ModelingToolkit.jl (MTK) enables researchers to formulate complex models in an easy-to-understand declarative manner. It can not only automatically lower those high-level models into efficient Julia code, along the way, MTK also optimizes differential-algebraic equations (DAEs) mathematically by reducing the number of algebraic equations and lowering the index of DAEs to 1. Those optimizations will drastically improve the simulation time of acausal models. In this talk, we will first talk about the motivation for using DAEs and acausal modeling before diving into the internal algorithms of MTK such as alias elimination, Pantelides algorithm, and tearing.

{{anchor symbolicarrays}}
* **Symbolic arrays: Past, Present and Future**

    *Time:* 12:20PM - 12:40PM

    *Speaker:* Shashi Gowda
 
    *Abstract:* In this talk, I will review previous work on expressing array operations in code and the manipulation of that code itself. I will consider trade-offs between loop-based programming and vectorized array operations (as in MATLAB), then explore newer developments in packages like JAX, Dex, XLA, and finally in Julia's Symbolics package. We explore how symbolic array operations with relevant metadata allows for optimization opportunities which are unavailable in straight-forward code.

{{anchor structuralid}}
* **Structural Identifiability Tools in Julia: A Tutorial**

    *Time:* 12:40PM - 1:00PM

    *Speaker:* Ilia Ilmer

    *Abstract:* In this tutorial, we will consider the problem of structural parameter identifiability, a property that can allow us to know in advance whether a model's parameters can be determined uniquely, up to finitely many values, or not at all. We will consider two Julia solutions to the problem, [SIAN.jl](https://github.com/alexeyovchinnikov/SIAN-Julia) and [StructuralIdentifiability.jl](https://github.com/SciML/StructuralIdentifiability.jl). Specifically, we will go over their basic functionality, comparison on several benchmarks, and how they can be used with other SciML packages such as [ModelingToolkit.jl](https://github.com/SciML/ModelingToolkit.jl).

{{anchor parallel}}
* **Parallel Extrapolation Methods for Differential Equations**

    *Time:* 1:00PM - 1:20PM

    *Speaker:* Utkarsh

    *Abstract:* Is there a way to parallelize serial ODE solvers where the Jacobian Matrix is too small to effectively parallelize in the LU-factorization stage? The answer is yes!

    This talk illustrates the novel multi-threaded extrapolation methods for solving stiff ODEs and investigates domains where serial solvers can benefit from multi-core machines by exploiting parallelism. We will demonstrate these techniques through representative applications and performance comparisons with pre-existing codes.

## Early-afternoon Section

**Chair:** Ranjan Anantharaman

{{anchor sponsor}}
* **Sponsor Talk by Julia Computing**

    *Time:* 1:30PM - 1:50PM

{{anchor udesbif}}
* **Learning measured bifurcation diagrams with UDEs**

    *Time:* 1:50PM - 2:10PM

    *Speaker:* Sandor Beregi

    *Abstract:* Nonlinear dynamical systems are frequently characterised by their bifurcation diagrams indicating the steady-state response as certain system parameters vary. This often involves multiple solutions corresponding to a single parameter-combination. We use universal differential equations (UDEs) to capture the dynamics accurately in such challenging parameter-domains whereas we also propose a boundary-value-problem-based approach to improve the robustness of the training procedure.

{{anchor udegaussian}}
* **Universal Differential Equations with Gaussian Processes**

    *Time:* 2:10PM - 2:30PM

    *Speaker:* Steffen Ridderbusch

    *Abstract:* In this talk we demonstrate using Gaussian Prosses as a basis for Universal Differential Equations, instead of Neural Networks.  As GPs, given the right underlying kernel, are also Universal Approximators, the combination promises to be similarly powerful and allows additionally for some quantification of the model uncertainty. This work connects the SciML and the JuliaGaussianProcesses ecosystems and enables interesting further research.

{{anchor udeepidemiology}}
* **Role of Universal Differential Equations in Epidemiology**

    *Time:* 2:30PM - 2:50PM

    *Speaker:* Raj Dandekar

    *Abstract:* Looking at Universal Differential Equations (UDEs) in the context of epidemiology, we answer the following questions : (a) Can UDEs be used to replace complex compartment models? (b) How robust is the UDE training procedure to varying neural network initializations? (c) Is symbolic recovery of missing epidemiological terms possible through UDEs? (d) How much data is required to train UDEs. Our proposed methodology is widely applicable in modelling diseases like Covid-19 and Influenza (H1N1).

## Late-afternoon Section

**Chair:**

{{anchor peds}}
* **Physics-enhanced deep surrogates (PEDS) trained end-to-end** (Invited Talk 2)

    *Time:* 3:20PM - 3:40PM

    *Speaker:* Raphael Pestourie

    *Abstract:* We present a physics-enhanced deep-surrogate approach towards developing fast surrogate models for complex physical systems described by  PDEs  and  similar  models: We propose a combination of a low-fidelity,  explainable physics simulator and a neural network that generates “coarsified” inputs, trained end-to-end to globally match the output of an expensive high-fidelity numerical solver.  The low-fidelity model ensures that governing conservation laws and symmetries are respected by design.

{{anchor fractional}}
* **Fractional Order Computing and Modeling with Julia**

    *Time:*  3:40PM - 4:00PM

    *Speaker:* Qingyu Qu

    *Abstract:* As the generalization of classical calculus and differential equations, fractional order calculus and differential equations are important areas that SciML has not supported, to provide a comprehensive Differential Equations package, we implemented many powerful FDE solvers. In this SciMLCon, we will talk about the progress we have taken in [FractionalDiffEq.jl](https://github.com/SciFracX/FractionalDiffEq.jl) and [FractionalCalculus.jl](https://github.com/SciFracX/FractionalCalculus.jl), how Julia helped us speed up fractional order modeling and computing,  and our plans to connect with SciML. 

{{anchor neuralplasma}}
* **Modeling Plasma Physics with NeuralPDE.jl**

    *Time:* 4:00PM - 4:20PM

    *Speaker:* Gabriel Birnbaum

    *Abstract:* Plasmas – the so-called fourth state of matter – are notoriously difficult to model. The equations that describe it are high dimensional and non-linear. In this talk, I will walk through how I built [Plasma.jl](https://github.com/killah-t-cell/Plasma.jl) – an application package that uses [NeuralPDE.jl](https://github.com/SciML/NeuralPDE.jl) to simulate plasmas with neural networks. I will share results and what I learned contributing to NeuralPDE, optimizing the solver for a specific application, and creating an intuitive interface.

{{anchor mixingimex}}
* **Mixing Implicit and Explicit Deep Learning with Skip DEQs**

    *Time:* 4:20PM - 4:40PM

    *Speaker:* Avik Pal

    *Abstract:* Implicit deep learning architectures separate the definition of a layer from the description of its solution process. While implicit layers allow features such as depth to adapt to new scenarios and inputs automatically, this adaptivity makes its computational expense challenging to predict. In this talk, we present a framework way to simultaneously achieve the robustness of implicit layers while allowing the reduced computational expense of explicit models.

{{anchor speeding}}
* **Speeding up x = A&#92;b with RandomizedPreconditioners.jl**

    *Time:* 4:40PM - 5:00PM

    *Speaker:* Theo Diamandis, Zach Frangella

    *Abstract:* We will introduce [RandomizedPreconditioners.jl](https://github.com/tjdiamandis/RandomizedPreconditioners.jl), a package for preconditioning linear systems using randomized numerical linear algebra. Crucially, our preconditioners do not require a priori knowledge of structure present in the linear system, making them especially useful for general-purpose algorithms. We will demonstrate significant speedups of positive semidefinite linear system solves, which appear in many machine learning and optimization problems.

{{anchor bifml}}
* **Bifurcation based machine learning of dynamical systems**

    *Time:* 5:00PM - 5:20PM

    *Speaker:*  Kyoung Hyun Lee

    *Abstract:* Combining scientific knowledge and machine learning, known as scientific machine learning (SciML), can improve the quality of the mathematical model in many cases. This research combines bifurcation theory with machine learning to model parameter-dependent nonlinear dynamical systems. Developed SciML methodology is applied to a real-world system with Hopf bifurcation and a harmonically forced electromagnetic system using Julia SciML packages.

{{anchor farewell}}
* **Farewell and Open Discussion**

    *Time:* 5:20PM - 6:00PM

    *Speaker:* Chris Rackauckas
