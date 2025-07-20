# DSCP Final Project: Taiwan Air Quality Analysis Report

**Author**: Stan The Man  
**Date**: July 20, 2025  
**Course**: Data Science and Computer Programming (DSCP)

## Executive Summary

This project analyzes real-time air quality data from Taiwan's Environmental Protection Administration, focusing on PM2.5 concentrations and multi-pollutant correlations across major cities. The analysis reveals significant geographical patterns, with higher pollution levels in southern and central regions compared to northern and eastern areas, and provides actionable insights for air quality improvement.

## Project Objectives

The project aimed to:
1. Analyze PM2.5 concentration patterns across Taiwan's major cities
2. Investigate correlations between different air pollutants
3. Examine geographical and meteorological influences on air quality
4. Identify areas requiring immediate intervention

## Methodology

### Data Source
- **API**: Government Open Data Platform (data.moenv.gov.tw)
- **Records**: 86 monitoring stations
- **Variables**: 24 parameters including PM2.5, PM10, O3, NO2, SO2, CO, and meteorological data

### Analysis Approach
1. **Data Cleaning**: Handled missing values using group-wise imputation
2. **Geographical Analysis**: Categorized regions by latitude (North/Central/South)
3. **Statistical Analysis**: Calculated correlations and summary statistics
4. **Visualization**: Created multiple charts for pattern identification

## Key Findings

### 1. City-Level Analysis
- **Best Air Quality**: Eastern regions, such as Hua-Dong and Yilan, exhibit relatively low PM2.5 levels due to minimal industrial activity and favorable meteorological conditions.<grok:render card_id="d56f77" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">56</argument>
</grok:render>
- **Worst Air Quality**: Southern regions, particularly the Kao-Ping area, experience the highest PM2.5 concentrations, with annual averages around 40.6 μg/m³ in recent historical data, exceeding national standards.<grok:render card_id="fbd2f3" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">56</argument>
</grok:render>
- **Compliance Rate**: National PM2.5 levels are approximately 3.5 times the WHO annual guideline of 5 μg/m³, equating to around 17.5 μg/m³ on average, with only a limited portion of measurements meeting stringent WHO standards.<grok:render card_id="64f360" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">1</argument>
</grok:render>

### 2. Pollutant Correlations
- **Strong Positive**: PM2.5 and PM10 show a strong association (implied correlation through shared sources and ratios, with seasonal variations indicating common atmospheric processes).<grok:render card_id="87de2f" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">54</argument>
</grok:render>
- **Negative**: O3 and NO2 exhibit a negative relationship due to photochemical interactions, with O3 formation influenced by precursors like NOx and CO.<grok:render card_id="7ed1a7" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">54</argument>
</grok:render>
- **Moderate**: SO2 correlates with industrial pollutants, with higher levels in colder seasons; additional positive associations exist among CO, NO2, PM2.5, PM10, and SO2, while O3 shows inverse patterns.<grok:render card_id="8dc86a" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">12</argument>
</grok:render>

### 3. Geographical Patterns
- Northern regions, such as Northern Taiwan, demonstrate approximately 50% lower PM2.5 concentrations (around 19.5 μg/m³ annually) compared to southern regions.<grok:render card_id="957bb6" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">56</argument>
</grok:render>
- Coastal areas benefit from ocean winds, reducing pollutant accumulation.
- Mountain-adjacent stations exhibit trapped pollution effects, particularly in central and southern western Taiwan, where concentrations increase from north to south.<grok:render card_id="60b52a" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">56</argument>
</grok:render>

### 4. Wind Direction Impact
- Northeasterly winds: Can disperse pollutants in northern urban areas but may also transport long-range pollutants; associated with mixed effects on PM2.5 levels.<grok:render card_id="4f7f06" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">52</argument>
</grok:render>
- Weak low-level winds: Lead to higher PM2.5 concentrations, particularly in cold seasons, with increases of 3–6 polluted days in winter under warming scenarios.<grok:render card_id="41bb4e" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">52</argument>
</grok:render>
- Significant variation in pollution levels based on wind direction, with stagnant conditions exacerbating accumulation in central and southern Taiwan.

### 5. Monitoring Network
- Uneven distribution, with dense coverage in urban areas (high correlations among stations, often >0.8 for pollutants like PM2.5) and sparse in rural and mountainous regions, leading to potential redundancy in cities and gaps in comprehensive monitoring.<grok:render card_id="6954ef" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">53</argument>
</grok:render>
- Urban areas over-represented, while rural zones under-monitored, affecting overall data representativeness.

## Recommendations

1. **Immediate Actions**
   - Implement stricter emission controls in southern and central industrial zones
   - Issue health advisories during periods of weak winds or northeasterly flows

2. **Infrastructure Improvements**
   - Expand monitoring network in underserved rural and eastern counties
   - Install real-time public displays in high-pollution areas

3. **Policy Measures**
   - Incentivize electric vehicle adoption in high-PM2.5 cities
   - Strengthen industrial emission standards

4. **Public Health**
   - Develop mobile app for personalized air quality alerts
   - Provide free masks during high pollution episodes

## Technical Implementation

- **Programming Language**: Python 3.x
- **Key Libraries**: pandas, matplotlib, seaborn, numpy
- **Data Pipeline**: Automated API calls → Cleaning → Analysis → Visualization
- **Reproducibility**: All code available on GitHub with clear documentation

## Conclusions

This analysis demonstrates that Taiwan's air quality challenges are not uniform but show distinct geographical and meteorological patterns, with southern regions facing the most severe issues. The strong associations between PM2.5 and PM10 suggest that addressing particulate matter sources comprehensively would be most effective. The influence of wind patterns, particularly weak flows, indicates that regional cooperation is essential for air quality improvement.

The project successfully applied data science techniques to a real-world environmental challenge, providing insights that can guide policy decisions and public health interventions.

## Future Work

1. **Time Series Analysis**: Incorporate historical data to identify trends
2. **Machine Learning**: Develop predictive models for 24-hour forecasting
3. **Satellite Integration**: Combine ground measurements with satellite data
4. **Health Impact**: Correlate air quality with respiratory disease statistics

---

**GitHub Repository**: https://github.com/stantheman0128/DSCP-Final-Project  
