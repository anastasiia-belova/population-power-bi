# Visualization in Power BI


## Final dashboards
![til](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/population_visualization.gif)

## Data

Source: provided excel files on online course

### Data Preparation

Data was cleared (NaNs filled, duplicates deleted, etc.) and transformed, e.g. some measurements a shown below.


![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_tables.PNG)

```
AveragePopulation = AVERAGE([Population])
```

```
FemalePopulation = CALCULATE(SUM([Population]), 'FACT-population'[Gender]="Female") 
```

```
FemalePopulationFilter = CALCULATE(SUM([Population]), FILTER('FACT-population',[Gender]="Female" && [Year]=1950)) 
```

```
ShareFemalePop = [FemalePopulation]/SUM('FACT-population'[Population])
```

```
TotalPopulation = SUM([Population])
```

```
DAX-test = CONCATENATE([Age-Grpoup],CONCATENATE(" ",[Age-Category]))
```

Below you can see final versions of tables

![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_table_age.PNG)
![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_table_region.PNG)
![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_table_population.PNG)

## Data Model

![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_data_model.PNG)

## Reports

### Examples of dashboards

In the screenshot below you can see different types of visualization (including different filters)

![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_dashboard_examples.png)

### Final dashboards

Finally dashboards were customized (colours, fonts, sizes, location)

![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_dashboards_in_process.PNG)
![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_final.PNG)

Below you can see dashboards closer

![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_dashboard_cards.PNG)
![Alt-текст](https://github.com/anastasiia-belova/population-power-bi/blob/main/pictures_population/pic_dashboard_map.PNG)

```python
# 

```

