# Neural network model and EDA for estimating obesity levels

main model file: `obesity_estimation_si.ipynb`

Exploratiory data analysis was made at the begining to determine what features are most important and to know their correlations.
Then quick check how random forest will perform (quite good actually - 93% acc). 
Next we were exploring which parameters will work best using Grid Search from `sklearn.model_selection` (very good tool).
At the end, we used the best parameters found to make a model and trained it on the training set which was 80% of the data (test set was ofc 20%) for 600 epochs.
On top of that using a scheduler to fine-tune the appropriate learinig rate for optimized learning.

**final accuracy**: 0.9314 - wchich is not bad at all

### Accuracy over epochs
![image](https://github.com/user-attachments/assets/feeb18ec-78c1-4e65-8838-30eb589b7c61)

### Tech stack
- env: conda
- pytorch (with CUDA)
- sklearn
- skorch 
- seaborn

### References
inspired by this paper: <br>
[Dataset for estimation of obesity levels based on eating habits and physical condition in individuals from Colombia, Peru and Mexico](https://www.semanticscholar.org/paper/Dataset-for-estimation-of-obesity-levels-based-on-Palechor-Manotas/35b40bacd2ffa9370885b7a3004d88995fd1d011#extracted)

link to the dataset:
https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition

### Citation and Credit

- Estimation of Obesity Levels Based On Eating Habits and Physical Condition  [Dataset]. (2019). UCI Machine Learning Repository. https://doi.org/10.24432/C5H31Z.
