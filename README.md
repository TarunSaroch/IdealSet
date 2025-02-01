> ### Disclaimer ⚠️
> The dataset provided has been synthetically generated using a Python script (available here) for educational and learning purposes only. All details, including names, locations, and personal information, are entirely fictional and do not represent real individuals or entities.

##
In today’s data-driven world, understanding how to work with realistic datasets is a crucial skill for students pursuing careers in data science, machine learning, and analytics. To support your learning journey, I’ve created a comprehensive synthetic dataset designed to simulate real-world scenarios while maintaining educational relevance.

### Dataset Description
The dataset consists of 25 attributes (columns) that describe various aspects of individuals. Below is a detailed breakdown of the table structure:

|Attribute|Description|Type|Example|
|---|---|---|---|
|`ID`|A unique identifier for each individual in the dataset.|Integer|1,2,3,...|
|`Name`|The full name of the individual.|String|"John Doe", "Jane Smith"|
|`Age`|The age of the individual in years.|Integer|25,30,52,...|
|`Gender`|The gender identity of the individual.|ENUM|"Male", "Female", "Non-binary", "Prefer not to say"|
|`DOB`|The date of birth of the individual.|Date|"1988-03-12", "1995-07-22"|
|`City`|The city where the individual resides.|String|"New York", "Tokyo", "Paris"|
|`Country`|The country where the individual resides.|String|"USA", "Japan", "France"-|
|`Income`|The annual income of the individual in USD.|Integer|60000.00, 120000.50|
|`Income_in_thousands`|Annual income in thousands.|Integer|60.00, 120.00|
|`Marital_Status`|The marital status of the individual.|ENUM|"Single", "Married", "Divorced", "Widowed"|
|`Employment_Status`|The current employment status of the individual.|ENUM|"Employed","Self-employed","Unemployed","Retired","Student"|
|`Num_Children`|The number of children the individual has.|Integer|0,2,1,...|
|`Education_Level`|The highest level of education attained by the individual|ENUM|"High School", "Bachelor", "Master", "PhD"|
|`Health_Status`|The self-reported health status of the individual.|ENUM|"Excellent", "Good", "Fair", "Poor"|
|`Height`|The height of the individual in meters.|Integer|1.75, 1.68|
|`Weight`|The weight of the individual in kilograms.|Integer|70.00, 60.50|
|`BMI`|Body Mass Index|Integer|23.85, 30.2|
|`Has_DL`|Indicates whether the individual has a driver's license.|Boolean|1 (True), 0 (False)|
|`Owns_Vehicle`|Indicates whether the individual owns a vehicle.|Boolean|1 (True), 0 (False)|
|`Blood_Group`|The blood group of the individual.|ENUM|'A+','A-','B+','B-','AB+','AB-','O+','O-'|
|`Smoker`|Indicates whether the individual is a smoker.|Boolean|1 (True), 0 (False)|
|`Alcohol_Consumption`|The frequency of alcohol consumption by the individual.|ENUM|"Never", "Rarely", "Often", "Ocassionally"|
|`Last_Physical_Checkup`|The date of the individual's last physical checkup.|Date|"2022-11-15", "2023-01-10"|
|`Email`|The email address of the individual.|String|"john.doe@gmail.com"|
|`Phone_Number`|The phone number of the individual|String|"+1234567890", "+819012345678"|
|`Allergies`|Any known allergies of the individual.|String|"None", "Pollen", "Nuts", "Shellfish",...|
|`Credit_Score`|The credit score of the individual, ranging from 300 to 900.|Integer|720, 650|
|`Life_Insurance`|Indicates whether the individual has life insurance.|Boolean|1 (True), 0 (False)|
|`Health_Insurance`|Indicates whether the individual has health insurance.|Boolean|1 (True), 0 (False)|

## What’s Wrong with the Dataset?
This dataset has been intentionally designed to include various imperfections and challenges commonly encountered in real-world data. Below is a detailed breakdown of the issues present in the dataset:

### 1. Missing Values Across Various Columns
Several rows contain missing values (`NULL` or `empty strings`) in key columns, simulating scenarios where data collection was incomplete or certain fields were left blank.

**Example of Affected Columns :** `Email`, `Phone_Number`, `Height`, `Weight`, `Age`, `Employment_Status`, `Education_Level`, and others.

### 2. Whole or Partial Missing Rows Representing Incomplete Data Collection
Some rows have multiple missing values across different columns (e.g., only `Name`, `Email`, or `DOB` are populated while other fields are   NULL  ). This represents cases where data collection was partially completed.

### 3. Inconsistencies for Outlier detection
**Inconsistent Age Values:** Negative ages (e.g., -5), ages greater than 150 (e.g., 200), and logically inconsistent ages (e.g., age < 0).
**Inconsistent Number of Children:** Negative values (e.g., -4) or unrealistically high numbers of children (e.g., 10).

### 4. Duplicate Records
The dataset contains duplicate rows, either exact copies or near-duplicates with minor variations (e.g., same `Name` and `Email` but different `ID`).
