# Cricket Performance Insight

# Motivation
To test my data scraping/analysis knowledge and take decisions on international cricket teams and players.

## Mission
This project tries to gather data from [ESPNCricinfo](https://www.espncricinfo.com/) to generate team and player statistics of the Bangladesh ODI cricket team, namely:
- Information of matches played in an arbitrary period of time.
- match stats of Bangladeshi players in each of those games.

This dataset was then analyzed to look for insight.

With little modification it can be used for other teams and other formats and other time periods.

## Scraping
Selenium was used to dynamically scrape the match links and the player statistics

## Wrangling
Dataset of each of the matches were wrangled to get:
- Match statistics (Win/Loss/Abandon/Stadium/VS/)
- Individual player statistics (Runs/Wickets/Econ etc)
- Captain statistics

## Analysis & key findings
This [Tableau Dashboard](https://public.tableau.com/shared/NZGC7FQHN?:display_count=n&:origin=viz_share_link) exposes the following key findings:

- Bangladesh consistently performs bad vs New Zealand.
- Jaker Ali and Nurul Hasan are consistently better than other batsmen
- Ebadot Hossain is consistently better at bowling than the rest of team, with relatively high wicket average, low economy
- Captain statistics were omitted due to homogeneity, Tamim Iqbal captained most of the games.


## Build
This python project was developed on windows.

```ps1
git clone https://github.com/chromaticv1/cricket_team_stats_analysis --depth=1
cd cricket_team_stats_analysis
python -m venv .venv
./.venv/scripts/activate
pip install -r requirements.txt
python src/main.py

```