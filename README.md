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

### Tool 1 (App Review)
|              	|    **PD &emsp;(bug report)** 	|       **RT &emsp;(rating)**     |     **FR &emsp;(feature request)**     |     **UE &emsp;(user experience)**     |
|:----------	|:---------------	|:---------------  |:---------------	|:---------------	|
|              	|    Pre&emsp;&emsp;Rec&emsp;&emsp;F1 	|       Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |     Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |     Pre&emsp;&emsp;Rec&emsp;&emsp;F1     |
|**SE domain (Poisson)** |      10.0%&emsp;37.5%&emsp;15.8%     |       72.1%&emsp;78.0%&emsp;74.9%  	|        7.1%&emsp;29.8%&emsp;11.5%     |      11.6%&emsp;32.0%&emsp;17.0%       |
|**SE domain (TF-IDF)** |      10.7%&emsp;40.2%&emsp;16.9%     |       72.2%&emsp;78.2%&emsp;75.1%  	|        7.9%&emsp;33.3%&emsp;12.8%     |      11.7%&emsp;32.5%&emsp;17.2%       |

### Tool 2 (RACK)
|              	|    **Top-10** 	|       **MRR@10**     |     **MAP@10**     |     **MR@K**     |
|:----------	|:---------------	|:---------------  |:---------------	|:---------------	|
|**SE domain (Poisson)** |     83.85%     |       52.29%  	|        43.27%     |      54.47%       |
|**SE domain (TF-IDF)** |      84.17%     |       53.20%  	|        45.82%     |      56.8%       |

### Tool 3 (Requirements Change Impact Analysis)
|              	|    **SE domain (Poisson)** 	|       **SE domain (TF-IDF)**     |
|:----------	|:---------------	|:---------------  |
|**Query 2**	|0.588	|0.588 |
|**Query 4**	|0.981	|0.981 |
|**Query 5**	|0.602	|0.602 |


### Overall Performance
| **Stop word list** | **Better**|**Worse** |**Same** |
|:----------	|:---------------	|:---------------  |:---------------  |
|No Stop Words|4 |12 |3 |
|[Very Small] (https://github.com/YaohouF/Stopwords/blob/main/stopwords_lists/very_small.txt)|10|7|2|
|**Small**|13|5|1|
|**Medium**|11|7|1|
|**Large**|11|8|0|
|**Technology Domain**|9|9|1|
|**SE Domain (Poisson)**|12|5|2|
|**SE Domain (TF-IDF)**|17|1|1|