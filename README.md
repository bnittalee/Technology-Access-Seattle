# Predicting Internet Access Among Low-Income Seattle Residents
<img src="https://github.com/bnittalee/Technology-Access-Seattle/blob/main/IMAGES/marvin-meyer-SYTO3xs06fU-unsplash.jpg" width="1000">
By Brittney Nitta-Lee

Date: April 21, 2023

# Introduction 
By providing technology access to low-income households, this project aims to bridge the digital divide in Seattle and offer opportunities to those who may otherwise be left behind. The final model, trained on a dataset from the City of Seattle, solves the problem with 97% accuracy.

# Business Understanding 
Seattle is a technology-driven city with existing research on digital equity and technology access, including data on the digital divide among low-income households. As an employee of a Public Housing Authority that serves low-income residents, I have witnessed firsthand the negative impact of a lack of technology access on individuals and their ability to participate in society. The motivation for this project is to contribute to ongoing efforts to address the digital divide and promote digital equity among low-income residents in Seattle.

# Data Understanding 
The data used in this project was obtained from the publicly available City of Seattle's Data Portal from 2018. The dataset comprises responses from a random survey of 4,315 Seattle residents. To focus on low-income residents, the analysis will concentrate on survey respondents whose household income is below $90,000, using the [2018 King County Income Limits from the U.S. Department of Housing and Development as a reference](https://www.huduser.gov/portal/datasets/il/il2018/2018summary.odn).

The dataset has certain drawbacks, such as a poor representation of Seattle's population, as the survey was administered only in English and Spanish, omitting speakers of other languages. This exclusion is unfortunate since data on technology accessibility among low-income residents who speak other languages could be highly informative.

The dataset comprises 479 columns, each containing binary data, and was gathered via a survey that involved responding to 38 questions. 

# Additional Resources 
[2018 Technology Access and Adoption Survey](https://github.com/bnittalee/Technology-Access-Seattle/blob/main/Data/Seattle%20IT%20Connectedness%20Study_Mail%20Version.pdf)

[Technology Access and Adoption Survey Codebook](https://github.com/bnittalee/Technology-Access-Seattle/blob/main/Data/Technology_Access_and_Adoption_Survey_2018_Codebook.csv)

# Data Collection 
A total of 4,315 surveys were collected from May 23rd through June 25th, 2018, representing 4,315 Seattle households and 10,358 Seattle residents.

- Conducted as a multi-mode survey: across mail, online, telephone, and in-person.

- Completed in both English (4,312 surveys) and Spanish (3 surveys).

- The overall average length of the online surveys was 34.0 minutes.

- The overall survey response was 18% (e.g. 18% of those invited to respond returned a survey).

All eligible respondents are:

- Individuals living within Seattle city limits; Able to conduct the survey in either English or Spanish;

- Has the ability to complete the survey via mail with paper and pencil or pen, online via computer, tablet, or smartphone, or in-person via paper and pencil or pen;

- Able to answer on behalf of the whole household on their use of technology and the internet (though if they needed help completing the survey, they could ask another household member or the survey helpline to assist them).

<center><img src="https://github.com/bnittalee/Technology-Access-Seattle/blob/main/IMAGES/Internet_access_1.png" width="500"></center>

There are 1483 households with internet access and 171 households without internet access. While the number of households with internet access is relatively low.

# Modeling
The baseline model that was used is a Logistic Regression model. The evaluation metrics that were used to compare with the advanced models are precision, recall, F1-score and accuracy. 

<img src="https://github.com/bnittalee/Technology-Access-Seattle/blob/main/IMAGES/Baseline_report_matrix.png" width="500">
