---
title: Data Science
tags: [DASCA, MBA]
style: fill
color: secondary
comments: true
description: Data Science
---

<!-- Start Document Outline -->
# Table of contents:
* [The Art &amp; Science of Driving Business](#the-art--science-of-driving-business)
	* [Part II. Data Science](#part-ii-data-science)
		* [Chapter 5. Differences Between Business Intelligence and Data Science](#chapter-5-differences-between-business-intelligence-and-data-science)
		* [Chapter 6. Data Science 101](#chapter-6-data-science-101)

<!-- End Document Outline -->

# The Art & Science of Driving Business
## Part II. Data Science
### Chapter 5. Differences Between Business Intelligence and Data Science


<table>
    <thead>
      <tr>
        <th colspan="2"></th>
        <th>Business Intelligence</th>
        <th>Data Science</th>
      </tr>
    </thead>
    
    <tbody>
      <tr>
        <td colspan="2">Definition</td>
        <td></td>
        <td>Data science is about finding <b>new variables and metrics</b> that are better predictors of performance</td>
      </tr>
      <tr style="background-color:#FFFFFF">
        <td colspan="2">Question</td>
        <td><li>Descriptive analysys, standard reports</li><li>What happended?</li><li>Low business value</li></td>
        <td><li>Predictive, prescriptive analysis: quantify causee and effect</li><li>Why, what is likely to happend, what should i do?</li><li>High business value</li></td>
      </tr>
      <tr>
        <td rowspan="7">Analyst characteristic</td>
        <td>Focus</td>
        <td>Reports, KPI, trend</td>
        <td>Patterns, correlations, models</td>
      </tr>
      <tr style="background-color:#FFFFFF">
        <td>Process</td>
        <td>Static, comparative</td>
        <td>Exploratory, experimentation, visual</td>
      </tr>
      <tr>
        <td>Data sources</td>
        <td>Pre-planned, added slowly</td>
        <td>On the fly, as needed</td>
      </tr>
      <tr style="background-color:#FFFFFF">
        <td>Transform</td>
        <td>Upfront, carefully planned</td>
        <td>In-database, on demand, enrichment</td>
      </tr>
      <tr>
        <td>Data quality</td>
        <td>Single version of truth</td>
        <td>"Good enough" probabilities</td>
      </tr>
      <tr style="background-color:#FFFFFF">
        <td>Data model</td>
        <td>Schema on load</td>
        <td>Schema on query</td>
      </tr>
      <tr>
        <td>Analysis</td>
        <td>Retrospective, descriptive</td>
        <td>Predictive, Prescriptive</td>
      </tr>
      <tr style="background-color:#FFFFFF">
        <td colspan="2">Analytics appoarches<br>(engagement process)</td>
        <td>
            <div>
            <img src="https://dungnv0696.github.io/nhathomongmer/assets/images/BI_analytic_approachs.png"/>
            </div>
            <div>
                Pre-build data model:
                <li>Identify all (or most) of the questions (1st, 2nd level questions)</li>
                <li>Work closely with data warehouse to build data model</li>
                <li>Schema onload</li>
                <br>
            </div>
            <div>
                Define the reports (query):
                <li>Use BI tool (Ex: SAP, cogmos, etc.) to create SQL-based query to build report</li>
                <li>Use graphical user interface (GUI)</li>
                <br>
            </div>
            <div>
                Generate SQL command:
                <li>After report is defined, BI tool create nesscessary commands</li>
                <br>
            </div>
            <div>
                Create report:
                <li>BI tool issues the SQL commands to make dashboard (interative process)</li>
            </div>
        </td>
        <td>
            <div>
                <img src="https://dungnv0696.github.io/nhathomongmer/assets/images/DS_analytic_approachs.png"/>
            </div>
            <div>
                Define hypothesis, prediction:
                <li>Define hypothesis, prediction to be made</li>
                <li>This is collaboration's result with business subject matter expert to understand key resources</li>
                <br>
            </div>
            <div>
                Gather data:
                <li>Gather relevant or potential interesting data from multiple sources, then push to DL or sandbox (collaboration)</li>
                <br>
            </div>
            <div>
                Build data model:
                <li>Schema on query: test several version before finding a schema that support model</li>
                <br>
            </div>
            <div>
                Visualize data:
                <li>Use visualization tool to find correlation, outliers</li>
                <li><b>Tableau, ggplot2</b>: use to indentify variables to test</li>
            </div>
            <div>
                Build analytics model:
                <li><b>SAS, SASMiner, R, Mahout, MADlib, Alpine Miner, H2O</b> to build model, try various techniques</b></li>
            </div>
            <div>
                Evaluate model:
                <li>Describe how well a model fit to observation: Kolmogorov-Smirnov, Person's, chi-square, ANOVA, confusion matrix</li>
            </div>
        </td>
      </tr>
      <tr>
        <td colspan="2">Data models</td>
        <td>
            Dimensional modeling (star schema):
            <ul>
                <li>Fact table:
                    <ul>
                        <li>Populated with metrics or measures</li>
                        <li>Correspond to transactional system</li>
                        <li>Numeric value</li>
                    </ul>
                </li>
                <li>Fact table:
                    <ul>
                        <li>Populated with attributes</li>
                        <li>Represent the "nouns" of transactional system</li>
                        <li>Group of hierachies and descriptors</li>
                        <li>Enable analytic exploration</li>
                    </ul>
                </li>
            </ul>
            <div>
            → Support nature question and answer exploration process (now standard to work with data warehouse)
            </div>
        </td>
        <td>
            Hadoop:
            <li>Provides oppotunity to think differently</li>
            <li><b>Written in Java, designed by Yahoo to deal with long, flat web logs</b></li>
            <li>Large datablock (64-128 MB) compare to ≤ 32KB by retional database</li>
            <li>Very long, flat records and long, flat data model (collapsing star schema into single flat record)</li>
        </td>
      </tr>
      <tr style="background-color:#FFFFFF">
        <td colspan="2">View of business</td>
        <td>Single version of truth or C360</td>
        <td>
            <li>Create analytic profile on each of organization's key business entity at individual level (ex: demographic, transactional metrics, social media metrics, etc.)</li>
            <li>Each analytic profile contains hundreds of metrics</li>
            <li>Depending on business initiative, some metrics may be more important than others</li>
            <div>
            Example of analysis process for improve customer retention:
            <img src="https://dungnv0696.github.io/nhathomongmer/assets/images/example_analysis_process.png"/>
            </div>
        </td>
      </tr>
    </tbody>
</table>

### Chapter 6. Data Science 101
![Advanced Analytic](https://dungnv0696.github.io/nhathomongmer/assets/images/advanced_analytic.png)

![Fundamental Exploratory Analysis](https://dungnv0696.github.io/nhathomongmer/assets/images/fundamental_exploratory_analysis.png)

### Chapter 7. Data Lake
Data lake can store:
- Structured data: relational table, csv files
- Semi-structured data: web logs, sensor logs, XML, json
- Unstructured data: text files, social media post, photos, videos
    
Data lake can do:
- Eliminate data silos: combine to single data lake
- Consolidate in efficient storage silos
- Provide a simple, scalable, plexible works across block, file, workloads. Improve operational flexibility
- Reduce IT cost, speed up time to insights
- Enable robust data protection
- Reduce data warehouse workload: moving Query to sandbox, datalake
- Free data warehouse by moving ETL to data lake
- Unhandcuff BI analyst, DS from being reliant on data warehouse as a single source

**If only focus on storing and ignore how or why data is used, governed, secured, data lake can turn into Data swamps**

Characteristics of a Business-ready data lake:
- Ingest: 
    - Rapidly ingest data from internal, external sources
    - Does not require any data transformation prior to
- Store:
    - Single/central repository for ALL data (even data is not used)
- Analyze:
    - Provide sandbox environment for DS
- Surface:
    - Support analytic model development and extract analytic result
- Act:
    - Enable integration of analytic result back to operational system, management system (close the loop)
    

<table>
<thead>
	<tr>
		<th>BI environment</th>
		<th>Analytics environment</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Create and deliver operational &amp; management report, dashboard on regular basis</td>
		<td>Exploratory environment, ingest and analyze a lot of data</td>
	</tr>
	<tr>
		<td>Predictable load</td>
		<td>Unpredictable load</td>
	</tr>
	<tr>
		<td>Service level agreement (SLA) constrained</td>
		<td>Experiment oriented: test data, algorithms, tools, techniques</td>
	</tr>
	<tr>
		<td>Heavily governed, historical data must be 100% accurate</td>
		<td>Loosely governed until it proves some value in data</td>
	</tr>
	<tr>
		<td>Standard tools</td>
		<td>Best tool for the job</td>
	</tr>
</tbody>
</table>

