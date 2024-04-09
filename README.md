# project-1


Data source: https://www.kaggle.com/datasets/catherinerasgaitis/mxmh-survey-results 
Author: Catherine Rasgaitis - Computer Science at University of Washington

Hypothesis:

    Null: There is no association between hrs per day listenign to music and mental health
    Alternative: There is a significant association between hrs spent per day and mental health

Data cleaning: Data was cleaned in the following ways: 

    Dropped unnecessary columns such as “Timestamp” and “Permissions”
    Dropped rows that were missing entries either “Age” or “Music effects”
    Removed “BPM” data that was clearly inaccurate and settled on scientifically noted range of  (<40 BPM or >300 BPM).
    Renamed around half the columns to be less redundant and easier to work with.

Data insights: 

    The streaming service were distributed across age groups with Spotify (64.3%) being most popular and majoirty 
    being the younger generation while Pandora is most commonly used by those 35 years of age and older. Rock is 
    the most popular music genre across all age groups. While popular genres did change by age group Rock, Pop, and
    Metal were consistently the choice across the board. A majority of participants are in their late teens to early
    twenties, mainly reflecting the modes of accessing the surveys ( social media played a key role in outreach).
    Having a background in music had little to no impact on the average severity of experienced mental health disorders

Submission by age:

    We wanted to get a general sense of the ages of users participating in the survey, so we created a box plot.
    The plot resulted in a Q1 of 18, a median of 21, and a Q3 of 27. Therefore, the majority of sumissions came
    from people in their late teens and early-mid 20s.
    
Musical background:

    Having a background in music, either playing an instrument or composing, does not change the impact that music
    has on mental health based on the mean of the self-reported severity of various mental disorders.
    
Self-reported effect of music on mental health:

    Even those that indicated that music does improve their mental health did not show a statistically significant
    increase or decrease in the severity of various mental health disorders. Without chronological data containing
    multiple mental health screenings, as well as corresponding data of the music listened to during that time period,
    we cannot confirm any long term or short terms effects music has on mental health.
    
Genre choices:

    Rock is predominantly the favorite genre across all age groups. Rock, pop, and metal were consistently the top
    three genre choices across all age groups, in various orders.
    
Improvement by Genre:

    After ordering all genres based on the likelihood of music benefitting mental health, we saw that all the genres
    were very close together, with classical being the least likely to benefit your mental health, and k pop being the
    highest. That being said, the sample sizes for some genres were low, and we would want to be careful about drawing
    conclusions.

Mental health vs BPM:

    We created a new column for a dataset that averages the 4 initial columns of "depression," "anxiety," "insomnia," and
    "OCD." We then used this averaged column of data to plot against the BPM of music that people listen to. Our scatterplot
    looked mostly random, and our p value came out to about 0.25, indicating that there is no statistical significance/
    correlation between BPM and mental health.

Music service:

    Next, we wanted to take a look at some data related to each user's primary streaming service. The options on the survey
    were Spotify, YouTube Music, Apple Music, Pandora, none, and other. First, we compared these music services against age.
    We were able to see which age demographics corresponded to which music services. Unsurprisingly, Spotify and Apple Music
    had the youngest age range, and Pandora had the oldest age range. This ties in with the next graph, which compares music
    service and mental health. For each music service, we calculated anxiety, depression, insomnia, and OCD scores. Spotify
    and Apple Music were at the top for anxiety, depression, and OCD, perhaps because those services are used by the younger
    demographic. Likewise, Pandora was significantly lower than the other music services in terms of all 4 ailments. Again,
    this could be because the older generations are the ones listening to that service.

Hours spent on music:

    Another thing we wanted to look at was how the amount of time someone spends listening to music is correlated with their
    self-perceived mental health. We broke down our ages into bins: 0-17, 18-25, 26-35, 36+. 

    There was a trend shown with the four age groups created with relation to hours spent listening to music - mainly trending downwards with age - the most hours were spent with the younger     age group and least amongst the oldest. Also the Mental Health trended with mainly older folks showing lower grades of the four ailments while these averages increased as the age             group got younger. And on the self reported Music effects - it was mainly positive towards music across the population set but again we couldn't conclusively confirm that many hours          hours on music translated to best mental health


Outcome: Conduct a controlled experiment where participants with some variation of mental health conditions are 'randomly' selected, and measure mental health outcomes (e.g., anxiety levels, depression scores) vs the amount of time spent listening to music (hrs) per day.

Interpretation of results and limitations:

  	The data set and analysis can not establish causation since there is inherent biases in the data source: see >> built in inherent biases in 'observational' data as opposed to a more dynamic dataset.
    The respondents provided their weight of mental Health ailments (self-reported) on a non scientific scale- a chronological study was not conducted to see if music helped overall well being after being introduced.
    The results show some remnants of a correlation between time spent listening to music and overall mental health, majority of the music per hours were spent by the younger age groups and Rock was the overall favorite genre of choice by all and across the age groups.
