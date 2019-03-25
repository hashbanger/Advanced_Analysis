## Models Log File

**Model 2**  
We dummified the variables *Age* and *Geography*.   
Accuracy - Increased  
Adjusted R Squared - Increased  

**Model 3**  
We removed the insignificant variables *HasCrCard* and *EstimatedSalary*.  
Accuracy - Increased  
Adjusted R Squared - Increased  

**Model 4**  
We tried removing the *Tenure* variable having not very high critical value for checking its effects on the model.  
Accuracy - Slightly Decreased  
Adjusted R Squared - Slightly Decreased  

**Model 5**  
We restore the model to *Model 3* by reselecting *Tenure* in our model.
Accuracy - Increased upto in Model 3  
Adjusted R Squared - Increased upto in Model 3  

**Model 6**  
We added a new variable *Log_Balance* i.e. Log transformed version of Balance and selected *Log_Balance* over *Balance*.  
Accuracy - Increased very slightly  
Adjusted R Squared - Decreased slighlty  

**Model 7**  
Added a new variable *Wealth_Accumulation* to calculate the *Balance* per unit *Age* increase and added new variable to the model.  
Accuracy - Almost same  
Adjusted R Squared - Decreased slightly  

**Model 8**  
Removed the *Log_Balance* variable as it has high collinearity with *Wealth_Accumulation* using the VIF.  
The significance of the *Wealth_Accumulation** increased from none to ***.  
The collinearity also decreased.     
Accuracy - Very slightly decreased  
Adjusted R Squared - Decreased slightly

**Model 9**  
Added a new variable *Log_WA = log10(Balance / Age +1)* added new variable to the model, also added *Log_Balance*, removed *Wealth_Accumulation*.  
Both *Log_Balance* and *Log_WA* became significant.  
Although the VIF are high through the roof for *Log_Balance* and *Log_WA*.  
Accuracy - Almost same  
Adjusted R Squared - Increased

**Model 10**  
Removed the *Log_WA*
Accuracy - Increased  
Adjusted R Squared - Slightly Decreased



***Model 10 is our final model considering all parameters and effects***