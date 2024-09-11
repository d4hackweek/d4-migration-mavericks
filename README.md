# Migration Mavericks

## Wildfire Migration project

This project focuses on addressing questions around migration and displacement of people and populations after wildfire events. Our research question include:

1. How are people displaced after a wildfire?
2. What ar ethe characteristics of those displaced?
3. What is the difference between mitigation efforts and capacity in places of origin and destination of displaced populations?



Provide a brief introduction describing the proposed work. Be sure to also decribe what skills team members will get to learn and practice as part of this project.

### Collaborators

| Name  | Role |
| ------------- | ------------- |
| Ethan | Project and Manuscript Lead |
| Mary Angelica | Project and Manuscript Champion |
| Sameer | Project Support and Manuscript Co-Author |

### The Problem


Provide a few sentences describing the problem are you going to explore. If this is a technical exploration of software or data science methods, explain why this work is important in a broader context and specific applications of this work.

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

*Validation on Migration - Independent Prediction*


Briefly describe and provide citations for the data that will be used (size, format, how to access).

### Existing methods

How would you or others traditionally try to address this problem? Provide any relevant citations to prior work.

### Proposed methods/tools

What new approaches would you like to implement for addressing your specific question(s) or application(s)?

Will your project use machine learning methods? If so, we invite you to create a [model card](model-card.md)!

### Additional resources or background reading

Optional: links to manuscripts or technical documents providing background information, context, or other relevant information.

## Project goals and tasks

### Project goals

We are interested in measuring accuracy and generating expected flows to possible destinations of migration and displacement due to wildfire events.

Project Data Goal: Production of three datasets: (1) origin migration; (2) destination dataset; (3) errors dataset

Goals Per Day:
* Day 1 (Monday)
- Begin project scoping

* Day 2 (Tuesday):
- Complete project scoping
- Draw outline of dataset production for the project
- Start data integration

* Day 3 (Wednesday):
- Data integration ~ disaster perimeter, displaced *N*
- Data integration ~ *a posteriori* predicted destinations
- Data integration ~ *a priori* predicted destinations
- Data integration ~ destination characteristics
- Work with floater on code for ML based classification from UC-CCP
- Draft slides (methods, challenges, and findings)

* Day 4 (Thursday)
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
