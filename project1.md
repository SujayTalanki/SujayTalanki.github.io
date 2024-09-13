## [Enhancing NanoGPT via Squentropy Loss and Hyperparameter Tuning](https://github.com/sujen07/NanoGPT-Loss-Stop-Analysis)
* [**Report of Findings**](https://github.com/sujen07/NanoGPT-Loss-Stop-Analysis/blob/main/DSC180BFinalReport.pdf), [**Website**](https://akshatm1011.github.io/Optimizing-NanoGPT/), [**Poster**](https://github.com/sujen07/NanoGPT-Loss-Stop-Analysis/blob/main/NanoGPTPoster.pdf)
* Formulated a custom and hybrid squentropy loss function to minimize empirical risk via PyTorch methods
* Created script to calculate model perplexity (metric that determines how "perplexed" a model is when predicting its next token; lower perplexity indicates better performance)
* Conducted large-scale hyperparameter tuning via distributed data parallel methods to attain 1.8 loss and 5.2 perplexity
* Hyperparameters tuned include learning rate, dropout rate, and number of layers
![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/a9dc6010-040a-4204-90b7-4530035587c5)
*Academic Poster of Findings*
![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/cc1a3a78-3ff8-49a5-8668-755d9d001545)
*Squentropy Loss Formula and PyTorch Code*
* Employed Python, numpy, pytorch, and pickle
