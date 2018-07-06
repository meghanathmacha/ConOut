# ConOut
Contextual Outlier Detection with Multiple Contexts. The work is accepted for publication and will appear in the proceedings of ECML PKDD 2018. 

## Website
https://cmuconout.github.io/  

## Requirements 
   * Requires [Jupyter](http://jupyter.org/) with R kernel to run the notebooks. Please follow this [guide](https://www.datacamp.com/community/blog/jupyter-notebook-r) if you are new to R.
   * Requires the following python packages:
```
numpy scipy pandas scikit-learn 
```
   * Requires the following R packages:
```
coin cluster stats factoextra dplyr corrplot
```

## File Structure 
1. The `data/` contains the public datasets used in the paper and `code/` contains two jupyter notebooks for each dataset. 
2. The pre processed features and labels are stored in the serializable RDS format in the `data/` folder. The type of the feature (categorical/numerical) is stored in the `typevar.RDS`
3. For a dataset, the `UnifiedMeasure` notebook (written in R) computes the unified measure and outputs the contexts and stores it as `context.RDS`
4. The `IsoForest` notebook (written in python) incorporates the contexts generated and computes the AUPRC. 

## Contact 
* Meghanath M Y (mmacha@cmu.edu) 
