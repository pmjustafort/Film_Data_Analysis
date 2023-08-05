# **Film Data Analysis**

## **Authors**:
Bobby Gerberick, Aung Si and Paul Justafort
![flat-lay-notebook-cinema-equipment](https://github.com/pmjustafort/Film_Data_Analysis/assets/137816262/b4d079d2-cabc-45d7-bd32-303efde3c061)

## **Overview**
Our film analysis project is a data-driven project that aims to uncover the key factors contributing to the financial success and popularity of movies in the cinematography industry.  This analysis project benefits from an extensive dataset comprising a staggering 146,000 films. This rich and diverse data was sourced meticulously from prominent film industry databases, including Box Office Mojo, Internet Movie Database (IMDB), Rotten Tomatoes, The Movie Database (TMDB), and The Numbers Movie Budget. By leveraging this comprehensive dataset, our project aims to gain valuable insights and provide data-driven recommendations to guide decision-making processes and optimize the success of movies in the ever-evolving and competitive film landscape.

## **Business Problem**
In the history of the cinematography industry, remarkable movies such as 'Avatar' (2009), 'Avengers: Endgame' (2019), 'Titanic' (1997), among others, have achieved tremendous success, captivating global audiences and redefining filmmaking. However, in the last years and amplified by the impact of the COVID-19 pandemic, the industry has faced significant disruptions due to the surge in popular streaming services like Netflix, Amazon Prime Video, Disney+, Tubi (which is free), Hulu, and others. As a result, producing a movie that attracts audiences to cinemas has become more challenging than ever before. Creating a successful film today requires unprecedented rigor and adaptation to the changing landscape of movie consumption.


## **Data**

For this project, we meticulously collected and cleaned comprehensive data from five prominent databases within the film industry: [Box Office Mojo](https://www.boxofficemojo.com/), [Internet Movie Database (IMDB)](https://www.imdb.com/), [Rotten Tomatoes](https://www.rottentomatoes.com/), [The Movie Database (TMDB)](https://www.themoviedb.org/), and [The Numbers Movie Budget](https://www.the-numbers.com/). From Box Office Mojo, we extracted valuable information on 3,387 movies released between 2010 and 2018, encompassing details such as title, studio, domestic gross, foreign gross, and year of release. IMDB proved to be an invaluable resource, supplying an extensive dataset covering over 146,000 movies with attributes like title, duration, rating, actors, directors, and writers. The Movie Database (TMDB) enriched our analysis with additional movie-related metadata, including posters, release dates, plot summaries, and production details. The Numbers Movie Budget contributed essential financial insights, including production budgets, domestic box office earnings, and worldwide box office earnings.
In order to ensure consistency and comparability, we carefully filtered and curated the data to create a sample of nearly 1500 films with the same set of variables we carefully filtered and curated the data to create a sample of nearly 1500 films with the same set of variables covering a window from 2010 to 2019. While we assessed data from all five sources, the primary data utilized in this project originated from Box Office Mojo, IMDB, and The Numbers Movie Budget. These datasets played a pivotal role in conducting a comprehensive analysis, encompassing both financial and qualitative aspects of the movies, resulting in meaningful conclusions and informed insights.


## Methods
In this project, a robust data processing approach was employed, which included eliminating rows with missing values to ensure data integrity. Additionally, numerical variables were standardized to achieve uniform scaling for unbiased analysis. Exploratory Data Analysis (EDA) was performed using Seaborn and Matplotlib, providing valuable initial insights, exploring data distributions, and identifying patterns. Tableau Public was utilized for the final visualization, creating interactive and visually appealing representations of the results. Multiple ANOVA tests were conducted to assess the significance of differences between variables, enabling a comprehensive understanding of various factors' impacts. Moreover, linear regression was applied to explore relationships between variables and potential predictors. Through these multifaceted methodologies, a systematic and thorough analysis was conducted, leading to valuable insights and sound conclusions derived from the dataset.

## **Data Understanding**

Our raw data had multiple common keys that allowed us to create a master dataframe contained director data, genre data, budget data, and revenue data. The final cleaned dataset ranged from 2010-2019, and we computed the ROI of each data entry as the ratio of profit (revenue minus budget)to budget.

## **Results**

[Genre ROI Distribution](./img/roi_boxplot_genre.png)

Our results show that the highest ROI genres were Mystery and Horror. These are low-bugdget genres that yield the highest relative profitability; on the more expensive end, Action and Adventure also yield a high ROI, though these require more production value and thus are more expensive to make. 

For Mystery and Horror, the two leading directors in these genres are Steven Soderbergh and Paul W.S. Anderson by ROI.

[Highest ROI Directors for Mystery and Horror](./img/mystery_horror_director_roi.png)

For Blockbusters, Bryan Singer takes the top seat.

[Highest ROI Directors for Blockbusters](./img/blockbuster_roi.png)

## **Conclusions**
Based on the analysis, several key factors have been identified that can significantly influence the success of your film project:
Budget Impact: The analysis suggests that budget plays a crucial role in the success of a film. Larger budgets are associated with higher expected box office gross. However, it is essential to note that higher budgets also come with increased risk. Therefore, filmmakers should carefully evaluate their financial resources and ensure that the budget aligns with the production's potential return on investment. While a larger budget may open doors to grander productions, it's equally essential to manage and optimize expenses to minimize risk.

Genre Selection: The analysis highlights the significance of choosing the right genre for a successful movie. Genres like animation, action and adventure, science fiction, and fantasy have been shown to be more profitable. Filmmakers should consider audience preferences, market trends, and the potential for the chosen genre to attract viewers and generate box office revenue. However, it's essential to maintain creativity and uniqueness within the chosen genre to stand out from the competition and engage the audience effectively.
The director's role is significant in shaping the film's overall quality and appeal. Collaborating with experienced and reputable directors can enhance the project's chances of success. Filmmakers should carefully consider a director's track record, style, and vision to ensure alignment with the project's objectives.

In conclusion, a successful film project requires a well-balanced approach that considers budget allocation, genre selection, and directorial expertise. By carefully managing budgetary constraints, strategically choosing popular genres, and collaborating with talented directors, filmmakers can increase the likelihood of realizing a successful movie with positive box office performance. However, it's crucial to maintain a balance between creative expression and commercial viability to resonate with the target audience and achieve both artistic and financial success.


## **Next Steps**
A data set of nearly 1500 films was used to derive these valuable insights and recommendations. However, it is important to acknowledge that having access to more data, especially concerning film budgets, could further enhance the accuracy and reliability of our recommendations. Having access to more comprehensive and accurate budget data would enable us to conduct more detailed analyses, resulting in better-informed decisions when it comes to allocating budgets and assessing risks, choosing genres, and directors.

This would significantly strengthen our ability to provide more tailored and effective recommendations to maximize the chances of a film's success. Therefore, in future endeavors, obtaining access to improved data sources would be an asset, enabling us to deliver even more valuable insights and strategies for creating successful films in the dynamic and competitive film industry. Therefore, in future analyses, obtaining access to improved data sources would be an asset, enabling us to deliver even more valuable insights and strategies for creating successful films in the dynamic and competitive film industry.

## **Further Details**

For a more comprehensive understanding, you can explore the full analysis in the Jupyter Notebook and access our interactive Tableau Dashboard which provides a comprehensive visual representation of the data, enabling deeper exploration and analysis.

## **Repository Structure**

Repository Structure:

|-- README.md
|-- LICENSE
|-- EDA (Rough).ipynb
|-- EDA (Final).ipynb
|-- .gitignore
|-- raw_data/
|-- img/
|-- cleaned_data/