---
layout: blog
title:  "Multivariate gaussian Distribution"
date:   2022-09-25 18:53:40 -0500
tags: probability detection
author: "Aniket Pramanik"
affiliation: "University of Iowa"
subtitle: "Hi welcome to Jekyll"
katex: True
---


Suppose we have a vector $\mathbf X \in \mathbb{R}^n$ such that
$$\mathbf X = \begin{bmatrix}
\mathbf x_1 \\
\vdots \\
\mathbf x_n
\end{bmatrix}$$
is a vector consisting of $n$ Gaussian distributed random variables $ \mathbf x_i \hspace{4pt} \forall \hspace{2pt} i \in \{1,2, \dots n\}$. $\mathbf X$ is called a Gaussian random vector with jointly Gaussian distributed random variable (r.v.) $\mathbf x_i \hspace{4pt} \forall \hspace{2pt} i.$

The probability density function (pdf) of a r.v. $\mathbf x_i$ is given as

$$f_{\mathbf x_i}(x_i) = \frac{1}{\boldsymbol \sigma_{\mathbf x_i} \sqrt{2\pi}} \exp\left( -\frac{1}{2}\left(\frac{x_i - \boldsymbol \mu_{\mathbf x_i}}{\boldsymbol \sigma_{\mathbf x_i}}\right)^2 \right) $$

where $\boldsymbol \mu_{\mathbf x_i}$ and $\boldsymbol \sigma_{\mathbf x_i}$ are mean and variance of $\mathbf x_i$ respectively.

$$
\mathbf x_i \sim \mathcal N(\boldsymbol \mu_{\mathbf x_i}, \boldsymbol \sigma_{\mathbf x_i}).  
$$

The pdf of $\mathbf X$ is given as,

$$
f_{\mathbf X}(x) = \frac{1}{|\boldsymbol \Sigma_{\mathbf X}| (\sqrt{2\pi})^N} \exp\left[ -\frac{1}{2}(\mathbf X - \boldsymbol \mu_{\mathbf X}) \boldsymbol \Sigma_{\mathbf X}^{-1} (\mathbf X - \boldsymbol \mu_{\mathbf X})^T \right]
$$

where $\boldsymbol \mu_{\mathbf X}$ and $\boldsymbol \Sigma_{\mathbf X}$ are the mean vector and covariance matrix of $\mathbf X$ respectively. $\|\boldsymbol \Sigma_{\mathbf X}\|$ denotes determinant of $\boldsymbol \Sigma_{\mathbf X}$.

$$
\mathbf X \sim \mathcal N(\boldsymbol \mu_{\mathbf X}, \boldsymbol \Sigma_{\mathbf X}).  
$$
