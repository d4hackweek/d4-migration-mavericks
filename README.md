# Migration Mavericks

## Wildfire Migration project

This project focuses on addressing questions around migration and displacement of people and populations after wildfire events. Our research question include:

1. How are people displaced after a wildfire?
2. What ar ethe characteristics of those displaced?
3. What is the difference between mitigation efforts and capacity in places of origin and destination of displaced populations?

Accurate population data are necessary for effective response and recovery after a disaster. Standard approaches to population estimation cannot necessarily be implemented after natural disasters, as they rely on systems that may be interrupted or unavailable. Disasters are growing in frequency and severity, magnifying an unmet need for tools to rapidly and accurately assess migration impacts of various sudden onset disasters. We compare several alternative methods for predicting migration destinations of displaced persons, and assess their performance in the case of two major wildfires in California. We plan on using datasets focused on population movements post-wildfire: the Camp Fire (2018) and Central Sonoma-Lake-Napa Unit (LNU) Complex Fires (2017).

Our project focuses on using Census demographic data, CalFire wildfire data, various datasets that measure migration, including University of California Consumer Credit Panel (UC-CCP). By integrating hazard (wildfire) data with demographic and migration data, we can begin to explain and simulate movement patterns of populations affected by wildfire. We also aim to understanding how (1) federal vulnerability measures map on to migration flows and (2) the efforts of hazard mitigation and community/government capacity in both places of origin and destination.

We used the D4 Hack Week to plan out data integration needs, list tasks for data and modeling needs, and established work flows for the needed analysis. We also used this time to explore issues with data integration, and learn more and incorporate machine learning to train a nueral network model to determine post-wildfire migration.

### Collaborators

| Name  | Role | Contributions |
| ------------- | ------------- | ------------- |
| Ethan | Project and Manuscript Lead | Data Integration and Model Building; Migration Assessments |
| Mary Angelica | Project and Manuscript Champion | Social Vulnerability, Governance Dimensions, Manuscript Planning, Data and Modeling Assessments |
| Sameer | Project Support and Manuscript Co-Author | Manuscript Development, Data and Modeling Assessments |

### The Problem

This project seeks to tackle understandings of wildfire-induced migration through data integration, behavior simulation (radiation and gravitational modeling), validate models, and build a neural network model.

The technical issues in exploring these data and modeling techniques is (1) incorporating both social and physical data at a variety of scales to the most granular model; (2) understanding behavior through different models while recongizing the need of validation of these movements; (3) find was to use machine learning techniques that are condusive with the data to better train simulation outputs to recognize possible migration patterns with robustness and rigor; (4) addressing roadblocks in assessing the social implication and governance capacity that lead to increased vulnerability for certain displaced populations.

Overcoming these obsticles to establishing sound modeling for simulated and realized migration flows has two potential positive outcomes:

1. Demographers and other social science researchers can work alongside climatologists, meteorologists, and other related weather researchers to develop similar models for understanding migration flows and displacement post-natural hazard.

2. Decision makers can used simulated models to better plan for migration flows, including investments in resources to location that may not have adaptable capacity to meet newly displaced populations.  

## Data and Methods

### Data

We will use the following datasets:
*Model Development*
1. Decennial Census Data:
   a. block-level population per household
   b. block-level vacancy rate
   c. block-level population
   d. population weighted centroids
2. CalFIRE Damage assessments reports dataset
3. CalFIRE Fire parameters

*Validation on Migration - Historical Data*
1. ACS PUMS
2. IRS Statistics of Income
3. LEHD/OTM

*Validation on Migration - "True" Data*
1. Parcel Data
2. NC-CCP Data

### Existing methods

- Geospatial analysis
- Post-hazard survey analysis

* Use of survey and surveillance data
   Fussell, E., Hunter, L. M., & Gray, C. L. (2014). Measuring the       
   environmental dimensions of human migration: The demographer’s toolkit. 
   Global Environmental Change, 28, 182–191. 
   https://doi.org/10.1016/j.gloenvcha.2014.07.001



How would you or others traditionally try to address this problem? Provide any relevant citations to prior work.

### Proposed methods/tools

- Neural Network
- Lessons from different disciplines
- 
What new approaches would you like to implement for addressing your specific question(s) or application(s)?

Will your project use machine learning methods? If so, we invite you to create a [model card](model-card.md)!

### Additional resources or background reading

Optional: links to manuscripts or technical documents providing background information, context, or other relevant information.

## Project goals and tasks

### Project goals

We are interested in measuring accuracy and generating expected flows to possible destinations of migration and displacement due to wildfire events.

Project Data Goal: Production of three datasets: (1) origin migration; (2) destination dataset; (3) errors dataset

Goals Per Day:
Day 1 (Monday)
- Begin project scoping

Day 2 (Tuesday):
- Complete project scoping
- Draw outline of dataset production for the project
- Start data integration

Day 3 (Wednesday):
- Data integration ~ disaster perimeter, displaced *N*
- Data integration ~ *a posteriori* predicted destinations
- Data integration ~ *a priori* predicted destinations
- Data integration ~ destination characteristics
- Work with floater on code for ML based classification from UC-CCP
- Draft slides (methods, challenges, and findings)

Day 4 (Thursday)
- Deliver slides

### Tasks

* Task 1 - Generate the total *N* displaced (for the total housing units in firezone or destroyed)
* Task 2 - Generate the actual total of *N* displaced
* Task 3 - Generate "a posteriori" family migrations (ACS, IRS, and LEHD data)
* Task 4 - Generate "a priori" parametric (gravity, raidation, and general radiation) (Siminietal 2012; Alis et al 2021)
* Task 5 - Generate NCOA flows (parcels > NCOALink > output > summarize)
* Task 6 - Generate UC-CCP flows (address within fire > COA > summarize)
* Task 7 - Assess prediction accuracy (Task 3 & 4 versus Task 5 & 6)

## Project Results

Use this section to briefly summarize your project results. This could take the form of describing the progress your team made to answering a research question, developing a tool or tutorial, interesting things found in exploring a new dataset, lessons learned for applying a new method, personal accomplishments of each team member, or anything else the team wants to share.

You could include figures or images here, links to notebooks or code elsewhere in the repository (such as in the [notebooks](notebooks/) folder), and information on how others can run your notebooks or code.
