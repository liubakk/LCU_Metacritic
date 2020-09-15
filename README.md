1.
Datascrapping using BeautifulSoup package from metacritic.com

metacritic_all_ea.ipynb
includes all titles from this page: https://www.metacritic.com/company/electronic-arts

metacritic_all_reviewed_titles.ipynb
includes all titles from this page: https://www.metacritic.com/browse/games/score/metascore/all/all/filtered?view=condensed

Data is stored in the following columns:
'DATE_ID','PUBLISHER','TITLE_URL', 'TITLE_NAME', 'PLATFORM','TITLE_GENRE', 'RELEASE_DATE_ID',
'METASCORE', 'CRITIC_REVIEWS_COUNT','POS_CRITIC_REVIEWS_COUNT','MIX_CRITIC_REVIEWS_COUNT','NEG_CRITIC_REVIEWS_COUNT',
'AGV_USER_SCORE', 'USER_RATINGS_COUNT', 'POS_USER_REVIEWS_COUNT','MIX_USER_REVIEWS_COUNT','NEG_USER_REVIEWS_COUNT'

Data clean-up
Titles excluded: mobile, missing metacritic score, not releases or cancelled.

Script optimisation
Python script includes a progress bar and outputs processing times for optimisation puposes.

2.
The data scrapped in then loaded into a Snowflake table using snowflake.connector
