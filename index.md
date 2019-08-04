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


### Week 10

...

Consider the samples $x_1, x_2, ..., x_n$. Draw samples with replacement until we have another set of samples $x_1, x_2, ..., x_n$. Thus it follows that the probability of choosing any one item is $\frac{1}{n}$ and the probability of not choosing this item is $1-\frac{1}{n}$. By independence of the samples, until the draw of $x_n$, we have the probability of not choosing any sample is $(1-\frac{1}{n})^n$. Now, if $n$ goes to infinity, the approximation of the original observations presented in each bootstrap sample is 
$$\lim_{n \rightarrow \infty } \Big(1- (1-\frac{1}{n})^n \Big)= \Big(1- \frac{1}{e} \Big) \approx 0.632$$

```markdown
Consider the samples $x_1, x_2, ..., x_n$. Draw samples with replacement until we have another set of samples $x_1, x_2, ..., x_n$. Thus it follows that the probability of choosing any one item is $\frac{1}{n}$ and the probability of not choosing this item is $1-\frac{1}{n}$. By independence of the samples, until the draw of $x_n$, we have the probability of not choosing any sample is $(1-\frac{1}{n})^n$. Now, if $n$ goes to infinity, the approximation of the original observations presented in each bootstrap sample is 
$$\lim_{n \rightarrow \infty } \Big(1- (1-\frac{1}{n})^n \Big)= \Big(1- \frac{1}{e} \Big) \approx 0.632$$

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/hdu214/sta314/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.


Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
