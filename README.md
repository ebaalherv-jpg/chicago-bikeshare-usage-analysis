# Chicago Bike-Share Usage Analysis

Analysis of Divvy bike-share trip data to understand behavioral differences
between members and casual riders in Chicago.

## Business Question
How does bike-share usage differ between members and casual riders, and
what does that reveal about customer segments and demand patterns?

## The Story

Chicago's Divvy system serves two very different riders: annual members
who treat it as daily transportation, and casual riders who treat it more
like a tourist experience. The data backs that up clearly — but the more
interesting story is *how* they ride, not just how often.

Members account for roughly 57% of all trips, and they lean far more
heavily on electric bikes than casual riders do — a pattern that holds
across nearly every station in the system, not just a handful of outliers.
That's a strong signal that speed and convenience matter more to a daily
commuter than to someone riding for leisure. Trip volume also follows a
clear weekly rhythm, with member and casual usage diverging between
weekdays and weekends.

Put together, these two patterns point to a concrete opportunity: casual
riders who already show member-like behavior — weekday e-bike trips
through commuter-heavy stations — are the strongest candidates for a
targeted membership upsell campaign.

## Tools
Tableau Public, CSV data (Divvy trip data)

## Key Findings
- Members account for roughly ~57% of trips, while casual riders make up the remaining share.
- Daily trip volume fluctuates in a weekly pattern, suggesting usage differs between weekdays and weekends.
- Electric bikes are used more heavily by members than by casual riders across nearly every station analyzed.

## Calculated Fields
   - `Duration (min)`: DATEDIFF('minute', [started_at], [ended_at])

## Dashboard
[View the interactive dashboard on Tableau Public] (https://public.tableau.com/views/EmilioAlfonso-CmosediferenciaelusodebicicletasentremiembrosyusuarioscasualesenChicago/EmilioAlfonso-CmosediferenciaelusodebicicletasentremiembrosyusuarioscasualesenChicago?:language=es-ES&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Data Source
Divvy trip data, publicly available at:
https://divvy-tripdata.s3.amazonaws.com/index.html
