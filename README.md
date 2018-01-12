# PharmIV_Stata

This respository supplies the Stata package to calculate the power of an instrumental variable analysis study using a single binary instrument Z to analyse the causal effect of a binary exposure X on a continuous outcome Y in the context of pharmacoepidemiology. If you use this material, please cite:

Walker VM, Davies NM, Windmeijer F, Burgess S, Martin RM. Power calculator for instrumental variable analysis in pharmacoepidemiology. Int J Epidemiol. 2017 Oct 1;46(5):1627–32. 

To find futher information relating to this paper, including the Stata code from the paper and the R package, please see https://github.com/venexia/PharmIV

## Stata package

This package can be used to calculate the power of an instrumental variable analysis study using a single binary instrument Z to analyse the causal effect of a binary exposure X on a continuous outcome Y. 

### Installation

```stata
net install github, from("https://haghish.github.io/github/")
github install venexia/PharmIV_Stata
```

### Syntax

The syntax for this package is as follows:

```stata
PharmIV, n(numlist) delta(numlist) alpha(numlist) sigma(numlist) prob_x1(numlist) prob_z1(numlist) cond_z1(numlist) cond_z0(numlist) 
```

### Example

What is the power of an instrumental variable analysis study with 10,000 participants to detect a treament effect of 0.20 for a treatment with a frequency of exposure of 0.50? The binary instrument for the study has a freqency of 0.20 and the probability of exposure given the instrument Z=0 is 0.57.

![alt text](https://github.com/venexia/PharmIV/blob/master/Screenshots/Stata_Example.png)
