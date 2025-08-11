6.Insights based on Non-Graphical and Visual Analysis:
Insights Based on Non-Graphical Analysis:
1. Director and Cast Information:
• By splitting the director and cast columns and analyzing them, we gain insights into
the diversity and frequency of collaborations in the film industry.
• Common directors and actors can be identified, allowing us to see patterns in movie
productions.
2. Duration Data:
• Extracting numeric values from the duration column provides a clear understanding of
movie lengths.
• Converting the duration to minutes allows for easy comparison and analysis across
movies.
3. Missing Values:
• Identifying and replacing missing values, such as replacing 'nan' with 'Unknown
director' and 'Unknown Actor', helps maintain data integrity and ensures that analyses
are not skewed by missing data.
• Replacing missing country data based on the director helps fill gaps and maintain
consistency in the dataset.
4. Data Binning:
• Creating bins for release years helps in categorizing movies into specific time periods,
making it easier to analyze trends over time.
• Binning allows for a more structured analysis of how movie characteristics (like
duration and rating) have changed over different periods.
Insights Based on Visual Analysis:
# 1. Distribution of Release Year:
• The histogram and KDE plot of the release year show the frequency of movie releases
over time.
• Peaks in the distribution can indicate periods of high production activity, while troughs
may indicate periods of lower activity.
# 2. Box Plots:
• Box plots for duration_minutes and release_year provide insights into the spread and
central tendency of these variables.
• Outliers identified in these plots can indicate unusual movie lengths or potentially
erroneous data entries for release years.
# 3. Correlation Heatmap:
• The correlation heatmap shows the relationship between duration_minutes and
release_year.
• Understanding these correlations helps in identifying trends, such as whether newer
movies tend to be longer or shorter.
# 4. Pair Plots:
• Pair plots provide a comprehensive view of the relationships between numerical
variables.
• Scatter plots within the pair plot can reveal linear or non-linear relationships, clusters,
and outliers.
• Histograms on the diagonal of the pair plot show the distribution of individual
numerical variables, highlighting any skewness or unusual patterns.
# Comments on the range of attributes
1. Director and Cast Information:
Range: The number of unique directors and cast members in the dataset.
Comments: The dataset likely includes a wide range of directors and actors, reflecting the
diversity of the film industry. Analyzing this range can highlight prolific directors and actors, as
well as collaborative networks.
# Duration (Minutes):
Range: The minimum and maximum duration of movies in minutes.
Comments: This attribute can vary widely, from short films to long feature films.
Understanding the range helps in categorizing movies into short, medium, and long durations,
and identifying any extreme outliers that might need further investigation.
# Release Year:
Range: The earliest and latest release years of the movies in the dataset.
Comments: The release years span a significant range, allowing for temporal analysis of movie
trends. The range indicates the historical depth of the dataset and can be used to study how
movie characteristics have evolved over time.
# Rating:
Range: The different types of ratings assigned to movies (e.g., G, PG, PG-13, R, etc.).
Comments: The range of ratings reflects the target audience and content suitability of the
movies. Analysing the distribution of ratings can provide insights into the types of movies
produced and their intended audiences.
# Country:
Range: The number of unique countries represented in the dataset.
Comments: A wide range of countries indicates a diverse dataset with international
representation. This range is crucial for understanding the global reach and cultural diversity of
the movies.
# Type (Movie/TV Show):
Range: The count of each type (movies and TV shows).
Comments: The distribution of movies versus TV shows can provide insights into the content
strategy of the platform or dataset source. A balanced range suggests a diversified content
offering.
# Date Added:
Range: The earliest and latest dates when the movies were added to the platform.
Comments: This range helps in understanding the platform's content acquisition timeline and
growth. It can also indicate periods of high content addition activity.
# Duration:
Range: The range of durations (typically in string format indicating hours and minutes).
Comments: When converted to numerical format, this range helps in analyzing the average
length of movies and identifying any trends in movie duration over time.
# Description:
Range: The length and content of movie descriptions.
Comments: The range of description lengths can vary, with some being short and concise,
while others are more detailed. Analysing these descriptions can provide insights into
marketing and content summarization practices.
# Comments on the distribution of the variables and relationship between them:
1. Distribution of Release Year
• Histogram Analysis:
The histogram of release years shows how the frequency of movie releases varies over time.
• Observations:
A) Peaks in the histogram may indicate periods of higher production, possibly reflecting
industry trends, technological advancements, or historical events.
B) Troughs may reflect periods of lower production.
C) Recent years often show higher frequencies due to increased production and digitization
of content.
• Skewness:
The distribution might be skewed towards recent years if the dataset includes more recent
entries.
2. Duration (Minutes)
• Box Plot Analysis:
The box plot of movie durations shows the central tendency and variability.
• Observations:
The median duration provides a typical length for movies in the dataset.
The interquartile range (IQR) shows the spread of the middle 50% of the data.
Outliers might indicate unusually short or long movies.
• Distribution Shape:
If the distribution of durations is not symmetric, it may be skewed. Long tails might indicate a
few extremely long movies.
3. Rating
• Categorical Distribution:
The count plot of ratings shows the frequency of each rating category.
• Observations:
A) Some ratings (e.g., PG-13, R) might be more common, reflecting target audience
preferences.
B) Less frequent ratings (e.g., G) could indicate fewer movies targeted at younger audiences.
• Implications:
Understanding rating distribution helps in analyzing the types of content that are predominant
in the dataset.
4. Year Bins
• Count Plot Analysis:
The count plot for binned release years shows the number of movies released in specific time
intervals.
• Observations:
A) Periods with high counts indicate more active movie production phases.
B) Analyzing these bins helps in identifying trends over time.
5. Country
• Geographical Distribution:
The frequency distribution of movies by country highlights the geographical diversity.
• Observations:
A) Some countries might dominate the dataset, reflecting major movie-producing regions
(e.g., USA, India).
B) Less frequent countries indicate regions with fewer productions or less representation in
the dataset.
Relationships Between Variables
1. Duration vs. Release Year
• Correlation Heatmap:
The heatmap shows the correlation between movie duration and release year.
• Observations:
A) A positive correlation might suggest that movie durations have increased over time.
B) A negative or no correlation indicates no clear trend in movie lengths over the years.
2. Pair Plot Analysis
• Pair Plots:
Scatter plots between numerical variables (e.g., duration, release year) provide insights into
their relationships.
• Observations:
A) Clusters or patterns in scatter plots might indicate trends or groupings in the data.
B) Histograms on the diagonal show the distribution of each variable.
6.3 Comments for each univariate and bivariate plot
Univariate Plots
1. Histogram of Release Year
Plot Description: A histogram showing the frequency distribution of movie release years.
Comments:
• The histogram highlights how movie production has varied over time.
• Observations: Peaks indicate years with higher movie production, possibly due to industry
trends, technological advancements, or cultural shifts.
• The distribution may show an increasing trend in recent years, reflecting the growth of digital
platforms and increased content production.
2. Box Plot of Duration Minutes
Plot Description: A box plot displaying the distribution of movie durations in minutes.
Comments:
• The box plot provides insights into the central tendency and spread of movie durations.
Observations: The median duration represents the typical length of movies in the dataset.
• The interquartile range (IQR) indicates the spread of the middle 50% of durations.
• Outliers represent unusually short or long movies, which might be worth investigating for
special genres or errors.
3. Count Plot of Ratings
Plot Description: A count plot showing the frequency of different movie ratings.
Comments:
This plot illustrates the distribution of content suitability ratings across the dataset.
Observations:
• Ratings like PG-13 and R might be more prevalent, reflecting the target demographics of the
movies.
• Less frequent ratings (e.g., G) suggest fewer movies aimed at very young audiences.
• Understanding rating distribution can help in identifying the predominant audience for the
content.
4. Count Plot of Year Bins
Plot Description: A count plot showing the number of movies released in specific time intervals (year
bins).
Comments:
• The count plot categorizes movie releases into defined periods, simplifying trend analysis.
• Observations: Periods with higher counts indicate active production phases, while lower
counts may reflect less activity.
• Binning helps in understanding how movie production has evolved over distinct time periods.
Bivariate Plots
1. Box Plot of Rating vs. Duration Minutes
Plot Description: A box plot comparing movie ratings and their durations in minutes.
Comments:
This plot reveals the relationship between content ratings and movie lengths.
Observations:
• Different ratings may have varying typical durations, reflecting genre tendencies and audience
preferences.
• For instance, longer movies might be more common in certain ratings, while shorter movies
could dominate others.
2. Correlation Heatmap (Duration Minutes vs. Release Year)
Plot Description: A heatmap showing the correlation between movie duration and release year.
Comments:
• The heatmap quantifies the linear relationship between these two variables.
• Observations: A positive correlation might suggest that movie lengths have increased over
time.
• A negative or weak correlation indicates no significant trend in movie durations with respect
to release years.
3. Pair Plot of Duration Minutes and Release Year
Plot Description: Pair plot showing scatter plots and histograms for duration and release year.
Comments:
• The pair plot provides a comprehensive view of the relationship between these numerical
variables.
• Observations: Scatter plots may show clusters or trends, while histograms reveal the
distribution shape of each variable.
• This visualization helps in identifying potential patterns, correlations, and outliers between
movie duration and release year.
7. Business Insights - Should include patterns observed in the data along with what you can infer
from it
Business Insights Based on Data Patterns
1. Temporal Trends in Movie Releases
Insight:
• There is a growing trend in movie production in recent years, likely due to the rise of digital
streaming platforms and advancements in filming technology.
• The movie industry is becoming more prolific, indicating a competitive market with numerous
releases annually.
2. Duration Patterns
Insight:
• Movies have varied durations, catering to different audience preferences and genre
requirements.
• Longer durations might indicate epic or detailed storytelling, while shorter ones could cater to
quick entertainment needs.
•
3. Content Rating Distribution
Insight:
• The dominance of specific ratings suggests a focus on content suitable for teenage and adult
audiences.
• Less frequent ratings like G indicate fewer productions targeted at very young viewers.
8. Recommendations - Actionable items for business. No technical jargon. No complications. Simple
action items that everyone can understand
Actionable Recommendations for Business
Increase Digital Presence:
• Focus on releasing more movies through streaming platforms like Netflix, Amazon Prime, and
Disney+. This will help reach a wider audience and adapt to the growing trend of online
viewing.
Diversify Movie Lengths:
• Produce a variety of movie lengths to cater to different viewing preferences. Offer shorter
films for quick entertainment and longer movies for in-depth storytelling.
Expand Family-Friendly Content:
• Increase the production of G-rated and PG-rated movies to attract families with young
children. This is an underrepresented market with potential for growth.
Invest in High-Profile Talent:
• Collaborate with well-known directors and actors to boost the appeal and marketability of new
releases. High-profile talent can draw larger audiences and enhance brand reputation.
Explore Emerging Markets:
• Expand production and distribution efforts in emerging markets such as Southeast Asia, Africa,
and Latin America. Tailor content to local cultures and preferences to gain a foothold in these
regions.
Monitor Viewer Feedback:
• Regularly collect and analyze viewer feedback to understand preferences and improve future
productions. Use surveys, social media, and streaming data to gather insights.
Promote Successful Collaborations:
• Highlight movies that involve successful director-actor partnerships. Use these collaborations
in marketing campaigns to attract fans and build anticipation.
Align Content with Trends:
• Stay updated with industry trends and audience interests. Produce content that reflects
current themes and popular genres to maintain relevance and attract viewers.
