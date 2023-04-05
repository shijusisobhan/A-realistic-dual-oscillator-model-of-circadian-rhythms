# A-realistic-dual-oscillator-model-of-circadian-rhythms
Circadian rhythms are biological oscillations with a period close to 24h, which modulates different physiological and behavioral processes in all the living organisms.In mammals, the circadian clock consists of activators ( Clock and Bmal1 ) that activates the repressors ( per and cry ), which in turn, after a delay, suppresses the activity of the activators and thereby inhibiting its own production. A single cell dual morning and evening oscillator was proposed by Daan et al., based on the molecular network that has two sets of similar non-redundant per1/cry1 and per2/cry2 circadian genes and each can independently maintain their endogenous oscillations.Here I am presenting a minimal mathematical model with the assumption that per1 gene acts a morning oscillator and per2 gene acts as an evening oscillator. For more details, please read the research article https://doi.org/10.1371/journal.pone.0177197

<img src="https://github.com/shijusisobhan/A-realistic-dual-oscillator-model-of-circadian-rhythms/blob/main/Picture1.jpg" align="center" width="600" height="700">

## ODE Model
The circadian model is based on ordinary differetial equations (ODE).We estimate all the parameters for the wild type by genetic algorithms to fit the mRNA’s and proteins got from the experiments. The present mathematical model consists of (i) Hill’s equation to describe the positive and negative regulations (ii) Michaelis-Menten equation to describe the degradation of mRNA’s and proteins (iii) mass action kinetics to describe both the complexation and first order degradation reactions. In the model, we also consider the nuclear and cytosolic per1/2 and Bmal1 genes and their proteins separately. The
variables Mp1, Mp2, P1c, P1n, P2c, P2n, Mb, Bc, BN, MR, R, PB1, and PB2, are per1 mRNA,
per2 mRNA, PER1 protein (cytosol), PER1 protein (nucleus), PER2 protein (cytosol), PER2
protein (nucleus), Bmal1 mRNA, BMAL1 protein (cytosol), BMAL1 protein (nucleus), Reverbα mRNA, REV- ERBα protein, PER1—BMAL1 complex, and PER2 -BMAL1 complex,
respectively. Rates are denoted by vsi (i = 1, 2. . .), Michaelis constants by kei’s, degradation constants by kdi’s, production and complexation rates by kpi’s, m and w are Hill’s coefficient to
denote co-operativity, kai’s denote activation constants, and kli denote inhibition constant.
L is the light parameter, which when silenced (L = 0), is taken to be under DD (No light) conditions.
There are overall 13 equations with 60 parameters

<img src="https://github.com/shijusisobhan/A-realistic-dual-oscillator-model-of-circadian-rhythms/blob/main/Picture3.jpg" align="center" width="500" height="700">

