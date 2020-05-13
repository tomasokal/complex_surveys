Chapter 1: Basic Tools
================
Tomas Okal
5/13/2020

# Key Points

  - A Probability Sample has 4 key components
      - All individuals in the target population must have a non-zero
        probability of ending up in the sample. This probability for
        individual ![i](https://latex.codecogs.com/png.latex?i "i") is
        ![\\pi\_{i}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bi%7D
        "\\pi_{i}").
      - This probability
        ![\\pi\_{i}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bi%7D
        "\\pi_{i}") must be known for every individual who ends up in
        the sample.
      - Every pair of individuals in the sample must have a non-zero
        probability of both ending up in the sample. This probability of
        both individuals ![i](https://latex.codecogs.com/png.latex?i
        "i") and ![j](https://latex.codecogs.com/png.latex?j "j") is
        ![\\pi\_{ij}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bij%7D
        "\\pi_{ij}").
      - This probability
        ![\\pi\_{ij}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bij%7D
        "\\pi_{ij}") must be known for every pair that ends up in the
        sample.
  - The fundemental idea behind design-based inference is that an
    individual sampled with a sampling probability
    ![\\pi\_{i}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bi%7D
    "\\pi_{i}") represents
    ![1/\\pi\_{i}](https://latex.codecogs.com/png.latex?1%2F%5Cpi_%7Bi%7D
    "1/\\pi_{i}") individuals from the target population. This value is
    the *sampling weight*.
      - Suppose a one individual sample from a target population
        ![N](https://latex.codecogs.com/png.latex?N "N") where each
        individual from that population might have a different sampling
        probability
        ![\\pi\_{i}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bi%7D
        "\\pi_{i}"). An estimate of some variable such as weight,
        height, or speed would be equal to the estimate of that
        ![i](https://latex.codecogs.com/png.latex?i "i") multiplied by
        ![\\pi\_{i}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bi%7D
        "\\pi_{i}"). Since it is based on only one individual, the
        population estimate may not be a good one, but it remains
        *unbiased*.
      - The Horvitz-Thompson estimator of the population total is the
        foundation for the analyses in the book. This estimator applies
        to any design, no matter how complicated, where
        ![\\pi\_{i}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bi%7D
        "\\pi_{i}") and
        ![\\pi\_{ij}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bij%7D
        "\\pi_{ij}") are known for the sampled observations. Further,
        the estimator depends on
        ![\\pi\_{ij}](https://latex.codecogs.com/png.latex?%5Cpi_%7Bij%7D
        "\\pi_{ij}") not just the sampling weights which is how the
        sampling design correlations are computed.
  - Different meanings of the term weights
      - A sampling weight of 100 means that that individual
        ![i](https://latex.codecogs.com/png.latex?i "i") represents 100
        individuals in the target population.
      - A precision weight of 100 means that that individual
        ![i](https://latex.codecogs.com/png.latex?i "i") has 100 times
        lower varaince than an individual
        ![j](https://latex.codecogs.com/png.latex?j "j") whose precision
        weight is 1.
      - A frequency weight of 100 means that the sample contains 100
        identical observations is being saved by using only one recode
        in the data to represent them all.
  - Design Effects
      - Defined by Kish, 1965 as the ratio of a variance of an estimate
        in a complex sample to the variance ofthe same estimate in a
        simple random sample.
      - Design effects will compare the variance from correct estimates
        in two different designs.
      - A design effect larger than 1 implies that larger sample sizes
        are needed for complex designs than for a simple random sample.
        This can still result in a lower overall cost.
