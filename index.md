<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>


## STA314 Statictical Methods to Machine Learning I

### Week 9

Question: 

Show that, for the maximum margin classifier, the correct value of $\beta_0$ is

### Week 10

Question:

In the lecture (and in the textbook) we learnt that "approximately $2/3$ of the original observations are present in each boostrap sample". This statement is only approximately correct. By computing the probability that each observation is present in a particular bootstrapped dataset, argue that, as the size of the training set
goes to infinity, a more precise number is $0.632 < 2/3$. Plot a graph of the number of samples in the training
data vs the expected proportion of unique observations in each data set, marking when it crosses $2/3$.


$Proof:$
Consider the samples $x_1, x_2, ..., x_n$. Draw samples with replacement until we have another set of samples $x_1, x_2, ..., x_n$. Thus it follows that the probability of choosing any one item is $\frac{1}{n}$ and the probability of not choosing this item is $1-\frac{1}{n}$. By independence of the samples, until the draw of $x_n$, we have the probability of not choosing any sample is $(1-\frac{1}{n})^n$. Now, if $n$ goes to infinity, the approximation of the original observations presented in each bootstrap sample is 
$$\lim_{n \rightarrow \infty } \Big(1- (1-\frac{1}{n})^n \Big)= \Big(1- \frac{1}{e} \Big) \approx 0.632$$


The following plot is a graph of the number of samples in the training
data vs the expected proportion of unique observations in each data set, which the training set contains 50 samples; also noting that it crosses the level of $\frac{2}{3}$, where the red horizontal line is at. 

![image](https://github.com/hdu214/sta314/blob/master/Rplot.png?raw=true)


