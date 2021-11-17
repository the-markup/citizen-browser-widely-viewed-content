# Citizen Browser: Facebook's Top Content
This repository contains data from the story "[Facebook Isn’t Telling You How Popular Right-Wing Content Is on the Platform](https://themarkup.org/citizen-browser/2021/11/18/facebook-isnt-telling-you-how-popular-right-wing-content-is-on-the-platform)" from from our series, [Citizen Browser](https://themarkup.org/citizen-browser/). 

The calculations underlying the article are detailed in our methodology, "[How We Investigated Facebook's Most Popular Content](https://themarkup.org/show-your-work/2021/11/18/how-we-investigated-facebooks-most-popular-content
)."

Citizen Browser construction and methodology is described in "[How We Built a Facebook Inspector](https://themarkup.org/citizen-browser/2021/01/05/how-we-built-a-facebook-inspector)."

## Data
The `data/` directory contains two subdirectories corresponding to analysis conducted on Facebook's Q2 and Q3 Widely Viewed Content reports.

Each subdirectory contains the following CSV files:
* `top20domains_fb_markup.csv` contains a list of the top 20 most viewed domains ranked by number of viewers, as provided by Facebook in its quarterly report. Additionally it contains two lists of the top 20 domains calculated by The Markup with Citizen Browser data, using the "Unique users" and "Impressions" metrics. 
The final column, "Rank change," shows the relative rank change of top domains under the "Impressions" metric compared with their ranks under the "Unique users" metric.

    This CSV is for human reference and is not optimally formatted for data processing.
* `unique_users-top-1000-domains.csv` contains the top 1000 domains from Citizen Browser data calculated by the number of unique users who were shown a link from the domain. This approximates the metric used by Facebook in its published domain rankings.
* `impressions-top-1000-domains.csv` contains the top 1000 domains from Citizen Browser data calculated by the number of impressions each domain received, i.e. counting the total number of times a domain was shown to each user, not just the number of users.