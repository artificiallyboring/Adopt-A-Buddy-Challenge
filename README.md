# Adopt A Buddy Challenge

![HackerEarth Challenge](/Image.jpg)

**Problem statement**

Having a pet is one of life’s most fulfilling experiences. Our pets spoil us with their love, compassion and loyalty. Thanks to social media, videos of clumsy and fussy (yet adorable) pets from across the globe entertain us all day long. Their love is pure and infinite. So, in return, all pets deserve a warm and loving family, indeed. And occasional boops, of course.

Numerous organizations across the world provide shelter to all homeless animals until they are adopted into a new home. However, finding a loving family for them can be a daunting task at times.  On International Homeless Animals Day, HackerEarth presents a Machine Learning challenge : Adopt a buddy.

The brighter side of the pandemic is an increase in animal adoption and fostering. To ensure that their customers stay indoors, a leading pet adoption agency plans on creating a virtual-tour experience, showcasing all animals available in their shelter. To enable that, a Machine Learning model is required to be built that determines type and breed of the animal based on its physical attributes and other factors.

**Dataset**

The dataset consists of parameters such as: a unique ID assigned to each animal that is up for adoption, date on which they arrived at the shelter, their physical attributes such as color, length and height, among other factors.

Precisely the dataset consists of the following items:

|   S. No.    | Column Name    |                     Description                 |
| :----       |    :----:      |                           :----:                |
|      1      | pet_id         | Unique Pet Id                                   |
|      2      | issue_date     | Date on which the pet was issued to the shelter |
|      3      | listing_date   | Date when the pet arrived at the shelter        |
|      4      | condition      | Condition of the pet                            |
|      5      | color_type     | Color of the pet                                |
|      6      | length(m)	     | Length of the pet (in meter)                    |
|      7      | height(cm)	   | Height of the pet (in centimeter)               |
|      8      | X1,X2	         | Anonymous columns                               |
|      9      | breed_category | Breed category of the pet (target variable)     |
|     10      | pet_category   | Category of the pet (target variable)           |

**Data Description:**

The data folder consists of 2 CSV files

* train.csv - 18834 x 11
* test.csv - 8072 x 9

*Sample Submission:*

| pet_id     | breed_category | pet_category |
| :---:      | :----:         |  :-----:     |
| ANSL_69903 | 0              | 1            |
| ANSL_66892 | 0              | 2            |
| ANSL_69750 | 2              | 4            |
| ANSL_71623 | 0              | 2            |
| ANSL_57969 | 0              | 1            |

**Evaluation Metric:**

> s1 = f1_score(actual_values[*'pet_category'*]), predicted_values[*'pet_category'*], average = *'weighted'*)

> s2 = f1_score(actual_values[*'breed_category'*]), predicted_values[*'breed_category'*], average = *'weighted'*)

> score = 100 x (s1 + s2)/2

**_Note:_** To avoid any discrepancies in the scoring, ensure all the index column values in submitted file matches the index column values in 'test.csv' provided.

*Time Limit*   :	5.0 sec(s) for each input file.

*Memory Limit* :	256 MB

*Source Limit* :	1024 KB
