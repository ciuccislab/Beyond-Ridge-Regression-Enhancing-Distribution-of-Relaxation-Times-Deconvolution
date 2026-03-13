# Beyond-Ridge-Regression-Enhancing-Distribution-of-Relaxation-Times-Deconvolution
This repository contains some of the source code used for the paper titled 'Beyond Ridge Regression: Enhancing Distribution of Relaxation Times Deconvolution' in the Journal of the Electrochemical Society, 171 (2024) 060529. https://iopscience.iop.org/article/10.1149/1945-7111/ad576a/pdf. The article is available online and in the docs folder.

Electrochemical impedance spectroscopy (EIS) is a characterization method often employed to investigate the physico-chemical properties occuring in electrochemical systems, such as batteries and fuel cells [1-2]. The success of EIS stems from its non-invasiveness, simplicity, and ability to probe a wide range of frequencies, and its main limitation is related to the analysis of the experimental data [3-5]. As an alternative to the standard equivalent circuits and physical models, the distribution of relaxation times (DRT) has gained a growing recognition to reliably identify physico-chemical processes in electrochemistry and beyond [1-2]. Typically, the DRT is deconvolved using the standard Tikhonov regularization, which minimizes the penalized distance between the experimental and DRT-based impedances using the Euclidean norm and the second-order differentiation matrix [7]. In this article, we investigate the influence of these two parameters and show how to robustify regularized regression, including when the data presents outliers, before we apply these results to real impedance data [9]. 


# Dependencies
numpy 

scipy

matplotlib

time

cvxopt

cxpy

bayes_opt


# Tutorials
1. **norm-DRT_distant2ZARC.ipynb**: this notebook shows how to deconvolve with different norms the DRT of impedance data artificially generated using two ZARCs in series;
2. **norm-DRT_SOFC.ipynb** : this notebook shows how to recover with different norms the DRT of real impedance EIS data measured by our group on a solid oxide fuel cell.

# Citation

```
@article{py2024beyond,
  title={Beyond ridge regression: Enhancing distribution of relaxation times deconvolution},
  author={Py, Baptiste and Ciucci, Francesco},
  journal={Journal of The Electrochemical Society},
  volume={171},
  number={6},
  pages={060529},
  year={2024},
  publisher={IOP Publishing}
}
```

# References

[1] Z. Wang, Y. Wang, F. Ciucci, Distribution of relaxation times: Foundations, methods, diagnostics, and prognosis for electrochemical systems, Curr. Opin. Electrochem. (2025) 101789. https://doi.org/10.1016/j.coelec.2025.101789.

[2] A. Maradesa, B. Py, F. Ciucci et al., Advancing electrochemical impedance analysis through innovations in the distribution of relaxation times method, Joule.  8 (2024) 1958-1981. https://www.cell.com/joule/fulltext/S2542-4351(24)00236-8.

[3] B. Py, A. Maradesa, F. Ciucci, Gaussian processes for the analysis of electrochemical impedance spectroscopy data: Prediction, filtering, and active learning. Electrochim. Acta. 439 (2023) 141688. https://doi.org/10.1016/j.electacta.2022.141688.

[4] B. Py, C. Zhao, F. Ciucci, Q. Meyer, Gaussian processes for fast and accurate measurements of the polarization resistance of hydrogen fuel cells from impedance spectroscopy, J. Electrochem. Society. 172 (2025) 074502.https://iopscience.iop.org/article/10.1149/1945-7111/ade82c/meta.

[5] B. Py, Z. Wang, Y. Wang, F. Ciucci, Entropy-based regularized regression for advanced distribution of relaxation times deconvolution, J. Power Sources. 644 (2025) 236910. https://doi.org/10.1016/j.jpowsour.2025.236910.

[6] T.H. Wan, M. Saccoccio, C. Chen, F. Ciucci, Influence of the discretization methods on the distribution of relaxation times deconvolution: implementing radial basis functions with DRTtools, Electrochim. Acta. 184 (2015) 483-499. https://doi.org/10.1016/j.electacta.2015.09.097.

[7] A. Maradesa, B. Py, T.H. Wan, M.B. Effat, F. Ciucci, Selecting the regularization parameter in the distribution of relaxation times, J. Electrochem. Society. 170-3 (2023) 030502. https://doi.org/10.1149/1945-7111/acbca4.

[8] M. Saccoccio, T.H. Wan, C. Chen, F. Ciucci, Optimal regularization in distribution of relaxation times applied to electrochemical impedance spectroscopy: ridge and lasso regression methods-a theoretical and experimental study, Electrochim. Acta. 147 (2014) 470-482. https://doi.org/10.1016/j.electacta.2014.09.058.

[9] B. Py, F. Ciucci, Beyond ridge regression: Enhancing distribution of relaxation times deconvolution, J. Electrochem. Society. 171 (2024) 060529. https://iopscience.iop.org/article/10.1149/1945-7111/ad576a/meta
