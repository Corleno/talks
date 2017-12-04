### Mathematically {data-transition="None"}

-   Composite *multivariate* function
    $$\mathbf{g}(\inputVector)=\mappingFunctionVector_5(\mappingFunctionVector_4(\mappingFunctionVector_3(\mappingFunctionVector_2(\mappingFunctionVector_1(\inputVector)))))$$

### Equivalent to Markov Chain {data-transition="None"}

-   Composite *multivariate* function

$$p(\dataVector|\inputVector)= p(\dataVector|\mappingFunctionVector_5)p(\mappingFunctionVector_5|\mappingFunctionVector_4)p(\mappingFunctionVector_4|\mappingFunctionVector_3)p(\mappingFunctionVector_3|\mappingFunctionVector_2)p(\mappingFunctionVector_2|\mappingFunctionVector_1)p(\mappingFunctionVector_1|\inputVector)$$

<object class="svgplot" data="../slides/diagrams/deep-markov.svg"></object>

### {data-transition="None"}

<object class="svgplot" data="../slides/diagrams/deep-markov-vertical.svg"></object>


### Why Deep? {data-transition="None"}

-   Gaussian processes give priors over functions.

-   Elegant properties:

    -   e.g. *Derivatives* of process are also Gaussian distributed (if
        they exist).

-   For particular covariance functions they are ‘universal
    approximators’, i.e. all functions can have support under the prior.

-   Gaussian derivatives might ring alarm bells.

-   E.g. a priori they don’t believe in function ‘jumps’.

### Process Composition


-   From a process perspective: *process composition*.

-   A (new?) way of constructing more complex *processes* based on
    simpler components.

*Note*: To retain *Kolmogorov consistency* introduce IBP priors over
latent variables in each layer.

### Analysis of Deep GPs {data-transition="None"}

-   [@Duvenaud:pathologies14] Duvenaud et al show that the derivative
    distribution of the process becomes more *heavy tailed* as number of
    layers increase.

-   [@Dunlop:deep2017] Theoretical analysis possible through conditional Gaussian Markov property.

### {data-transition="None"}

<object class="svgplot" data="../slides/diagrams/deep-markov-vertical.svg"></object>

### {data-transition="None"}

<object class="svgplot" data="../slides/diagrams/deep-markov-vertical-side.svg"></object>

