# Interactive Probabilistic Models Explorer (IPME)
An interactive visualization explorer of the model graphs and inference results of probabilistic models expressed in probabilistic programming languages (PPLS). 
Intented for interactive exploration of the uncertainty of Bayesian probabilistic models and enhancement of their interpretability. 
It takes as an input a zip file (.npz). This file contains a description of the model's structure along with the inference results (MCMC samples) 
in a standardized form of a collection of npy arrays and metadata. 
For example, the [arviz_json](https://github.com/johnhw/arviz_json) package creates this standardized output of probabilistic models expressed in PyMC3.

# Examples
The examples directory includes some examples of use based on the output of some Bayesian probabilistic models specified and run in PyMC3.
The examples are organized per problem. Each problem's directory includes a Python code file, model.py, 
demonstrating the specification of the problem's model and the export of the inference data into 
the standardized format described above. There is another Python code, ipme.py, which demonstrates 
the use of the ipme package for the transformation of the model's output into an interactive multiverse diagram.
Note: For the specification and run of the PyMC3 models, you need to install PyMC3, ArviZ, and the arviz_json package.  
