# Stopwords
This repository is intended as an example of how the stopwords are produced and to provide the data used in the paper (Stop Words for Processing Software Engineering Documents: Do they   Matter?)

## Folder Structure
```
Stopwords
    |_ data_for_replications (contains all the required data for replicating software engineering tools)
       |_ Maalej_Dataset (original data for app review tool)
       |_ queries (queries used for RACKTool)
    |_ stackoverflow_questions (more than 10k top reviewed questions on stackoverflow)
    |_ stopwords_lists (all the stoplists)
    |_ replications
    |_ stackoverflow (code for creating the domain-specific corpus)
```
## Expected Result
The result may vary by a small fraction depending on the trial, but it should be approximately the same as the tables below.

|              	|    **PD &emsp;(bug report)** 	|       **RT &emsp;(rating)**     |     **FR &emsp;(feature request)**     |     **UE &emsp;(user experience)**     |
|              	|    Pre&emsp;&emsp;Rec&emsp;&emsp;F1 	|       Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |     Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |     Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |
|:----------	|:---------------	|:---------------  |:---------------	|:---------------	|
|              	|    Pre&emsp;&emsp;Rec&emsp;&emsp;F1 	|       Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |     Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |     Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |
|**SE domain (Poisson)** |      10.0%&emsp;37.5%&emsp;15.8%     |       72.1%&emsp;78.0%&emsp;74.9%  	|        7.1%&emsp;29.8%&emsp;11.5%     |      11.6%&emsp;32.0%&emsp;17.0%       |