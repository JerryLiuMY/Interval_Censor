# Bayesian Inference on Plackett-Luce Model
<p>
    <a href="https://cran.r-project.org/package=Seurat">
        <img src="https://www.r-pkg.org/badges/version/Seurat"
            alt="python"></a> &nbsp;
    <a href="https://opensource.org/licenses/MIT">
        <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
            alt="MIT license"></a> &nbsp;
</p>


- The article considers a progressive three-state model with states 1, 2, 3 and two possible transitions: 1 → 2 and 2 → 3. The time of 1 → 2 transition (S) is interval censored and the time of 2 → 3 transition (T) is either interval censored or right censored. The process may also be right censored in state 1.

- The authors propose methods for finding the nonparametric maximum likelihood estimator (NPMLE) of the joint distribution F(s,t) of S and T from doubly interval censored (DIC) data. They adapt an algorithm by Maathuis (2005) to obtain the support rectangles and develop a new algorithm to estimate the probability masses.

- Two nonparametric tests of the Markov property are developed for the DIC model:

  - An extension of Kendall's coefficient of concordance that uses imputation to handle incomparable observation rectangles.
  - An adaptation of a logrank-type statistic proposed by Titman and Putter (2022) that uses the estimated probabilities of the maximal intersection rectangles.

- Under the Markov assumption, S and T should be conditionally independent given the current state. The tests assess this at different times t conditional on being in state 2 at time t.

- The methods are applied to an AIDS dataset involving times of HIV infection and AIDS onset, both of which were interval censored. The tests do not provide evidence against the Markov assumption for this dataset.
The authors note that the developments could be extended to an interval-censored illness-death model that allows a direct 1 → 3 transition in addition to the 1 → 2 and 2 → 3 transitions.

In summary, the article proposes NPMLE and hypothesis testing methodology for evaluating the Markov assumption in a progressive three-state model with interval censoring, and illustrates the approach on data from an AIDS study.
