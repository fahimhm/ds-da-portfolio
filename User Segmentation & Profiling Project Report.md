# User Segmentation & Profiling Project Report

## Project Title: Customer Segmentation and Persona Development From Their Online Activity

Author: Fahim Hadi Maula  
Date: September 6th, 2025. 
Notebook: [here](./clustering%20model%20scratch.ipynb)



### Executive Summary

This report details a data-driven user segmentation and profiling project for a hypothetical advertising company. The primary goal was to move beyond generic marketing and gain a deeper understanding of our user base. By applying K-Prototypes clustering to behavioral data, we successfully identified three distinct user segments: the **Engaged Urban Professionals**, the **Information Seekers**, and the **Mobile-First Passive Users**. For each segment, a detailed persona was developed, outlining their unique behaviors, motivations and pain points. The finding from this analysis will inform targeted marketing campaigns, personalize product recommendations, and optimize the overall user experience, ultimately driving increased revenue and customer loyalty.

### Project Objective

The objective of this project was to perform a comprehensive analysis of user data to:

1. **Identify** distinct and meaningful user segments.

2. **Profile** each segment based on their behaviors and characteristics.

3. **Provide** actionable recommendations to improve business outcomes.

### Data & Methodology

#### Data Sources

The analysis was conducted on a dataset containing 1,000 anonymized user records. The data was sourced from [statso.io](https://statso.io/2024/02/25/user-profiling-case-study/).

#### Feature Engineering

Raw data was transformed into a set of features suitable for clustering. Key features included:

- Numerical Features (Standardized):
    - Likes and reactions
    - Followed accounts
    - Time spent online (weekday)
    - Time spent online (weekend)
    - CTR
    - Conversion Rates
    - Ad Interaction Time
    - Number of interested topics
- Categorical Features (One-Hot Encoded):
    - Age
    - Location
    - Education level
    - Device usage
    - Income level
    - Individual interest topics

#### Methodology

We used **K-Prototypes Clustering**, an unsupervised machine learning algorithm, to group users into segments. This algorithm was chosen because it effectively handles both numerical and categorical data within the same model. The optimal number of clusters (<i>k</i>) was determined using the **Elbow Method**. This process indicated that a solution with 3 clusters provided the most balanced and interpretable segmentation.

![Elbow Method](assets/Elbow%20Method.png)

### Segmentation Analysis & Personas

Based on our analysis, we identified three core user segments. For each segment, a detailed persona was created to provide a human-centric view of the data.

#### Segment 1: The Engaged Urban Professional

**Summary:** This cluster is defined by its high level of online engagement and diverse interests. Users in this group spend more time interacting with ads and have the highest conversion rates, indicating that the are not only active but also highly receptive to advertising.

- **Key Characteristics:**

    - **Size:** $34.6\%$ of the user base.
    - **Demographics:** Predominantly young to middle-aged adults (25-44 years old) with a wide range of educational backgrounds and higher income levels, with a significant portion earning over $$80,000$. They are most likely to live in urban areas and primarily use desktop devices.
    - **Behavior:** High number of followed accounts and frequent likes and reactions. They have high CTR, conversion rates, and ad interaction time.
    - **Top Interests:** This group's interests are broad and span a variety of topics, showing the highest interest levels across all categories. Their top interests include:
    
        - Investing and Finance ($26.01\%$)
        - Music Production ($25.43\%$)
        - Digital Marketing ($23.12\%$)
        - Gourmet Cooking ($22.25\%$)
        - Fitness and Wellness ($22.54\%$)
        - Gaming ($21.97\%$)
        - Reading and Literature ($22.54\%$)

    - **Persona:** "Alex, The Urban Professional"

        - Alex works in a fast-paced environment. He values tools that are reliable and powerful. He doesn't have time to deal with bugs or poor design. He is a high-value user who is receptive to ads for professional services, productivity tools, and business-focused content.

#### Segment 2: The Information Seeker

**Summary:** This group is less directly engaged but is crucial for content reach. They are characterized by their primary use of search functions to find specific information or answers, rather than extensive browsing.

- **Key Characteristics:**

    - **Size:** $33.8\%$ of the user base.
    - **Demographics:** This group has a balanced age distribution, with a slight concentration in the 25-34 age group. Their education and income levels are diverse, and they are evenly distributed across different locations and device-types, though they show a slight preference for mobile-only usage.
    - **Behavior:** Users in this cluster are characterized by a high click-through rate (CTR), meaning they frequently click on ads, but have a lower interaction time and conversion rate compared to Segment 1. This behavior suggests they are curious and actively seek out information, but are more selective about their purchases.
    - **Top Interests:** Their online presence is very active, with a high number of followed accounts. While they are interested in various topics, their interest levels are more moderate compared to Cluster 0. Their top interests include:

        - Digital Marketing ($18.34\%$)
        - Eco-Friendly Living ($17.75\%$)
        - Fashion Modelling ($17.46\%$)
        - Gourmet Cooking ($16.57\%$)
        - Software Engineering ($16.27\%$)
        - Pet Care ($15.09\%$)
        - Travel and Adventure ($15.38\%$)
    
    - **Persona:** "Sarah, The Knowledge Seeker"

        - Sarah is a student or researcher who is always looking for quick facts and reliable sources. She uses search engines to navigate directly to the content she needs. She is open to educational ads, but will ignore anything that doesn't directly address her current query.

#### Segment 3: The Mobile-first Passive User
**Summary:** This segment's engagement is casual and mobile-centric. They are often browsing passively and highly influenced by visual content.

- **Key Characteristics:**

    - **Demographics:** This group is well-distributed across age groups, with a notable number of older users (55−64 years old). They primarily use a combination of mobile and desktop devices. They have a lower number of followed accounts and lower likes and reactions, suggesting a more passive or selective online presence. Their income and educational backgrounds are varied.
    - **Behavior:** This cluster shows the lowest overall engagement with ads, as indicated by a lower CTR and less time spent on ads. This group has the most focused interests, with the majority of users following only one or two topics. Their interest levels across all specific topics are consistently the lowest among the three clusters. Their online activity is also more moderate compared to the other clusters, with more activity on weekdays and less on weekends.
    - **Persona:** "Mark, The Casual Scroller"

        - Mark uses his phone to unwind in the evening. He scrolls through his favorite apps and is influenced by eye-catching video ads and influencer content. He is not interested in complex features and prefers a simple, intuitive user experience.

### Strategic Recommendations

Based on the segment profiles, here are actionable recommendations for different business functions

| Segment                   | Marketing Recommendations         | Product Recommendations          |
|---------------------------|-----------------------|-----------------------------|
| Engaged Urban Professional | - Create campaigns for professional services and premium feature.<br>- Send personalized emails with curated product recommendations.<br>- Offer early access to new tools as an exclusive reward. | - Prioritize development of features that enhance productivty.<br>- Ensure a seamless, high-performance desktop experience.<br>- Collect feedback from this group to guide product roadmap. |
| Information Seeker        | - Optimize content for search engines (SEO).<br>- Create sponsored articles or informative blog posts.<br>- Use text-based ads that link to relevant answers or resources. | - Improve the search functionality and filtering options.<br>- Develop a clear and organized knowledge base or FAQ section.<br>- Minimize pop-ups and intrusive ad placements. |
| Mobile-first Passive User | - Focus on social media and influencer marketing.<br>- Use short-form video ads and visually engaging content.<br>- Run mobile-only campaigns with simple calls to action.  | - Ensure the mobile app is highly optimized and user-friendly.<br>- Develop a visual discovery feed similar to social media platforms.<br>- Gamify some features to increase engagement. |

### Future Research

For future research, it's recommended to explore alternative approaches to clustering and dimensionality reduction to gain a more comprehensive understanding of the dataset.

- **Exploring DBSCAN for Density-Based Clustering:** It would be valuable to apply a **density-based clustering algorithm** like **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** to the dataset. Unlike traditional methods like k-means, DBSCAN can discover clusters of arbitrary shapes and is effective at identifying noise or outliers. This is particularly useful if the clusters in your data are not spherical or if you suspect there's a significant amount of noise. By comparing the results of DBSCAN with your current distance-based approach, you can better determine which method is more suitable for the data's inherent structure.

- **Evaluating Data Structure with Dimensionality Reduction:** To make a more informed decision between distance-based and density-based clustering, it's highly recommended to first apply **dimensionality reduction techniques**. **Principal Component Analysis (PCA)** and **t-SNE (t-Distributed Stochastic Neighbor Embedding)** are excellent choices for this.

    - **PCA** is a linear method that identifies the principal components—the directions of maximum variance in the data—which can help you understand the overall data structure and reduce noise.

    - **t-SNE** is a non-linear technique that is particularly effective at visualizing high-dimensional data by mapping it to a 2D or 3D space.  The resulting visualizations can provide crucial insights into whether the data forms distinct, well-separated groups (which might favor a distance-based method) or exhibits more complex, intertwined, or dense regions (suggesting a density-based approach like DBSCAN is more appropriate).