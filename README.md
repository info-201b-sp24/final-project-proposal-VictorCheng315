# Final Project Proposal

## Project title

Data-Driven Analysis of Dog Adoption in the U.S

### Authors

Victor Cheng, Le Luo, Rain Hou, Cindy Xu.
### Date

April 30th, Winter 2023
## Abstract

This project aims to analyze the data of adoptable dogs in the US, collected from the PetFinder API on a single day. The focus will be on understanding the distribution and characteristics of these dogs, and how these factors might influence their chances of adoption.

## Keywords

Adoptable Dogs, Animal Shelter, Animal Welfare

## Proposal

1. Introduction  

In our daily lives, we still see stray pets on the streets, which sparked our interest in the current situation of animals in pet shelters. After searching the Internet, we found that until today, animal adoption is still a big topic that needs attention. We believe that our project can provide some help to improve the current situation of stray animals and shelter animals. The purpose of this project is to better understand the adoption of dogs and other animals in the United States. We are curious about how the characteristics of shelter animals affect their chances of being adopted, and how these characteristics varied by location. By analyzing the data of adoptable dogs, we can gain insight into the characteristics of these dogs and how they affect their chances of being adopted. We hope that the results of this project can help shelters and rescue agencies so that they can optimize their efforts to find homes for these dogs.

 The research questions are:

What are the most common breeds among adoptable dogs?

Is there a correlation between age or size and adoption rates?

How do the characteristics of dogs vary across different states?

Does the color of the dog influence its chances of adoption?

2. Related Work  

Our topic is the adoption pattern across the US.

One related work is about predicting and minimizing the animal length of stay in a shelter and euthanization. According to this research article, size, and adoption rates. The result of that study shows that younger and smaller animals tend to have higher adoption rates compared to older and larger ones, which is likely due to the perception that younger and smaller animals are easier to manage and adapt better to new environments.
Citation: Bradley, Janae, and Suchithra Rajendran. “Increasing Adoption Rates at Animal Shelters: A Two-Phase Approach to Predict Length of Stay and Optimal Shelter Allocation - BMC Veterinary Research.” BioMed Central, BioMed Central, 5 Feb. 2021, bmcvetres.biomedcentral.com/articles/10.1186/s12917-020-02728-2#citeas.

The second article we find discusses how a dog’s coat color influences its stay at a shelter and the likelihood of it being reclaimed. Brindle and multicolor dogs have the shortest length of stay (LOS) at shelters, while black dogs stay the longest. Coat color doesn’t significantly affect the time lost dogs spend at a shelter before being reclaimed, which typically happens within a day. The study suggests that black, brown, and brindle dogs are more likely to be abandoned, while fawn, black and tan, grey, and red dogs are more likely to be reclaimed if lost.
Citation: Voslarova, Eva, et al. “Coat color of shelter dogs and its role in dog adoption.” Society &amp; Animals, vol. 27, no. 1, 4 Jan. 2019, pp. 25–35, https://doi.org/10.1163/15685306-12341491.

The topic of this related research paper is to examine the factors affecting the decision-making of prospective dog owners. It concludes that human-related factors like prior ownership experience, age, gender, income, and education impact preferences. Demographics such as gender, age, and income predict acquisition sources. Social trends affect breed choices. Dog-related factors like appearance and temperament significantly influence decisions, with appearance often prioritized over health, especially among certain breed owners like French Bulldogs. However, studies show limitations, with retrospective data and correlation-based findings lacking causality. Further research is needed to understand the interaction of these factors precisely and develop tools for responsible acquisition practices and promoting canine welfare.
Citation: Holland, Katrina E. “Acquiring a Pet Dog: A Review of Factors Affecting the Decision-Making of Prospective Dog Owners.” Animals : An Open Access Journal from MDPI, U.S. National Library of Medicine, 28 Mar. 2019, www.ncbi.nlm.nih.gov/pmc/articles/PMC6523466/.

3. The Dataset

> Where did you find the data? Please include a link to the data source  

https://github.com/the-pudding/data/tree/master/dog-shelters

> Who collected the data?  

Amber Thomas

> How was the data collected or generated?

All data except for description was collected using PetFinder’s V2 API method get-animals as described in their documentation. Since the V2 API doesn’t return the full animal description, the creator of this dataset was encouraged by the API maintainers to query the same animal profiles using the V1 API to acquire that information. Thus, the creator used all of the shelter ID’s returned from the V2 API calls to find all descriptions of dogs in each shelter and combine the two results by the animal’s unique ID.  

> Why was the data collected?  

The data was collected to provide a snapshot of the adoptable dogs in the US.

>How many observations (rows) are in your data?  

There are 58,180 rows in this dataset.

> How many features (columns) are in the data?

There are 36 columns in this dataset.

> What, if any, ethical questions or questions of power do you need to consider when working with this data?  

Ethical considerations include ensuring the privacy and confidentiality of the shelters and rescues that posted the dogs for adoption.

> What are possible limitations or problems with this data?   (at least 200 words)

The dataset only represents some information about adoptable dogs in the US on a single day, which means that the data might not accurately represent the overall trend of adoptable dogs in the US. Seasonal variations, special events, or other temporal factors that might influence the number and characteristics of adoptable dogs are not captured in this dataset.

Another potential limitation is the bias caused by the self-reported data. Because the information about the dogs is reported by the shelters or rescues that posted the dogs for adoption on PetFinder. The accuracy and completeness of this information depend on the individual shelters or rescues, which might vary widely. Some shelters or rescues might provide detailed and accurate information about the dogs, while others might provide minimal or inaccurate information. This could introduce biases in the data and affect the reliability of the analysis.

Moreover, the dataset is limited to dogs listed on PetFinder. Although PetFinder is a popular platform, we all know that not all shelters or rescues might be using this platform. Therefore, there might be regional variations in the use of PetFinder, with some areas having a high proportion of their adoptable dogs listed on the platform, while others might use different platforms or methods for listing their adoptable dogs. This could limit the comprehensiveness of the data and introduce geographical biases in the analysis.

4. Implications

The potential impact of this study is manifold, starting with the enhancement of technology platforms. For individuals involved in the design and technology of platforms such as PetFinder, the findings from this study can provide important insights that shape the development of new features. These characteristics can be especially helpful in promoting animals that are often overlooked in the adoption process, such as older animals or specific breeds. The second is about strategies for public engagement and education. In addition to influencing policy and technology, insights from this research may also be critical in advancing public engagement initiatives. Educational campaigns can be designed to change public perceptions and encourage more diverse adoption options. By educating the community about the needs and benefits of adopting less popular breeds, these events may lead to a shift in adoption patterns and improved outcomes for these animals.

5. Limitations & Challenges

First of all, the sample data of this study is too large, which requires everyone to spend a lot of time analyzing during the research process. Another very important point is that only the size of single-day data can be analyzed, and the trend cannot be analyzed. For example,  Analyzing data from only a single day limits the ability to discern longer-term trends and patterns. This approach might miss seasonal variations, longer-term shifts in data, or emerging trends that develop over time. For a more comprehensive analysis, it’s crucial to include data spanning longer periods to capture a broader spectrum of influences and outcomes. There might be potential biases in the data, as it is based on the information reported by the shelters or rescues. Deliberately not providing data, these situations will lead to bias in the final results.The reliability of the data could be compromised by biases introduced through selective reporting or inconsistencies in how data is collected and reported by different shelters or rescues. Such biases can skew the analysis, leading to conclusions that may not accurately reflect the true situation. Ensuring data consistency and addressing potential sources of bias are essential for accurate research findings.

Acknowledgements

We would like to thank everyone in this team as we all put a real effort into this project.
