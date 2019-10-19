# dantools
some useful snippets and tidbits

A general place to leave code and interesting thoughts or research.

Reduce memory in your pandas dataframe (I think I only like the float64 to float32, unless it's categorical (the uint8 preferences can be killer if you accidentally have one value in the set you use, say if you groupby to small groups): 
https://www.mikulskibartosz.name/how-to-reduce-memory-usage-in-pandas/

Or good one: https://medium.com/@vincentteyssier/optimizing-the-size-of-a-pandas-dataframe-for-low-memory-environment-5f07db3d72e

For example, this 2nd place TwoSigma kaggler says your models should have at most parameters less than the log of your data... ?

https://www.kaggle.com/c/two-sigma-financial-news/discussion/102914#latest-610467
Krzysztof Urbanowicz
•
(2nd in this Competition)
•
2 months ago
Thank you Corey, this was for sure team work. One more comment related overfitting, which I think, was the case of all models, that there is a simple rule of thumb. This rule is simple saying that number of degrees of freedom (here number of parameters) should not be larger, or even should be much smaller than natural logarithm of number of data. This is becuase with logarithm one can calculate dimension of system and this is relevant to number of degrees of freedom. In such case relevant is to say "keep it simple".
