# SWSR: A Chinese Dataset and Lexicon for Online Sexism Detection

## Overview

Our repository presents the first Chinese sexism dataset -- **Sina Weibo Sexism Review (SWSR) dataset** -- containing sexism-related posts collected from Sina Weibo platform, as well as a large Chinese lexicon **SexHateLex**. The SWSR dataset can be exploited for building computational methods to identify and investigate online, gender-related abusive language. The SexHateLex lexicon can also support detection and analysis of sexist contents.

Please find more details in our [paper work](https://www.sciencedirect.com/science/article/abs/pii/S2468696421000604) and earlier released dataset versions [here](https://doi.org/10.5281/zenodo.4773875).

## Data Format

### SWSR Dataset

SWSR dataset consists of two files:  `SexWeibo.csv` and `SexComment.csv`, corresponding to 1,527 weibos and 8,969 comments.

**SexWeibo.csv**

* weibo_id: a string of weibo ID
* weibo_text: a string of weibo text
* keyword: contains  the  sexist  keyword(s)  extracted  from  the weibo. Not every weibo has corresponding keyword(s) 
* user_gender: the gender of user
* user_location: the location of user
* user_follower: number of users who follow this user's account
* user_following: number of users whom this user follows
* weibo_like: number of like for the weibo
* weibo_comment: number of comment for the weibo
* weibo_repost: number of repost for the weibo
* weibo_date: the date and time when the weibo is posted
                

**SexComment.csv**

* weibo_id: the weibo id where the comment is collected
* comment_text: a string of comment text 
* gender: the gender of commenter
* location: the location of commenter
* like: number of like for this comment
* date: the date and time when the comment is posted
* label: the comment is sexist(1) or non-sexist(0)
* category: categorise sexism into four classes -- Stereotype based on Appearance(SA), Stereotype based on Cultural Background (SCB), MicroAggression (MA) and Sexual Offense (SO)
* target:  the type of target who are attacked -- Individual (I) or Generic (G)

### SexHateLex Lexicon

The SexHateLex lexicon contains a list of 3,016 abusive and sexist terms in `SexHateLex.txt`.

## Reference

Our work has been published in the Journal of Online Social Networks and Media. If you are interested in this dataset, please cite: 

```
Aiqi Jiang, Xiaohan Yang, Yang Liu, Arkaitz Zubiaga, 
SWSR: A Chinese dataset and lexicon for online sexism detection, 
Online Social Networks and Media, 
Volume 27, 
2022, 
100182, 
ISSN 2468-6964, 
https://doi.org/10.1016/j.osnem.2021.100182.
```

If you have any queries or suggestions about our work, please contact us via aiqi.jiang@yahoo.com. We also welcome any ideas or cooperation about online abuse especially gender-based abuse and cross-lingual scenarios.
   


