# Trash Data Model

## Context
The State Water Board’s Office of Information Management and Analysis (OIMA) is developing a new method to monitor and assess the quantity, distribution, and makeup of trash on streets to better understand the amount of trash entering (or being prevented from entering) California’s water bodies. OIMA has been working on a pilot project in partnership with the City of West Sacramento to develop a proof-of-concept tool that identifies and classifies trash in images using a customized computer vision model for trash identification, built on open-source machine learning resources and trained using a large library of images gathered from a street sweeper-mounted camera pointing at street curbs and gutters.

## Management Questions
- How much trash is entering our water bodies?
- What type of trash is in the waters?
- What can we learn by analyzing trash data over space and time?

## Problem
While a data model has been developed, there is plenty of more work to do! We need to streamline the current data model, develop a corresponding data schema, and develop a way to integrate (1) data across temporal and geographic scales and (2) monitoring methods for trash, debris and microplastics, etc.

## 2019 California Water Boards Science Symposium: Water Science Datathon
### Challenge Questions
DATA MODEL: 
- How would you revise/improve upon the data model?
- What else would be interesting to incorporate into the data model?  
- What information is needed to make a more robust and accurate data model for trash identification and classification?
- How do we integrate data across spatial and geographic scales?
- How do we integrate the varied monitoring methods for trash, debris, microplastics, etc.?

DATA SCHEMA: 
- How do we go from a data model to a useful data schema?
- What kinds of fields are present in each table and how they are organized?
- How are the fields in each table defined (e.g. data types and definitions)?

### Potential Challenge Tasks
Add to or revise the current data model. 
- Develop a list of elements to add, and how to link them to the rest of the data model. 
- Develop a list of elements to remove from data model, if necessary. 
- Define organization, relationships, and dependencies among data elements.

Develop data schema
- Define tables (what fields are in each table?)
- Define fields within each table (What are the data types and definitions for each field?)

Develop a list of data gaps. What data do we need to move forward on this project?

Provide an update on the project. How far did you get? What challenges did you face? How did you overcome these challenges or what do you need to do so?

### Datathon Debrief
- The team identified gaps in the current data model, debated the merits of several different approaches to filling those gaps, and evaluated proposed taxonomies. At the same time, they weighed network (flat) taxonomic models and hierarchical models for trash classification, sought to address gaps in site characterization, and focused on calculated trash density as a vehicle for interoperable comparisons of trash presence across various methods. The team also briefly discussed the ability for the data model to accommodate derived data products such as statistics from machine learning algorithms, counts from imagery, and other synthetic, aggregated datasets.
- Next steps will be to continue to iterate on the project to further refine the data model and schema. Additionally, there needs to be a validation of the appropriate classification system for trash. The Data Management subcommittee of the Trash Monitoring Workgroup will adopted as its charge the task of detailing how the model can accommodate derived data.

## Resources
California Water Board West Sacramento Street Sweeper Project
- GitHub Repo: https://github.com/CAWaterBoardDataCenter/Trash-Tracker
- See Trash_Test_Images Folder for example images from the project. 
- The model and data structure is in progress. In terms of the characteristics we’d like to identify for each piece of trash, we are aiming to use a schema called COMB, which stands for Category, Object, Material, Brand. Essentially this means identifying each piece of trash with a label for all four of those features. For now we will probably ignore the Category part (because we are still defining what that means in our context), but we’d like to have the model be able to provide the following information for each piece of trash:
  -	Object: the type of object, for example cup, bottle, wrapper, cigarette, straw, etc.
  - Material: what it’s made of, e.g. paper, plastic, aluminum, cardboard, glass, etc.
  - Brand: probably not available in many cases, but in some cases it may be identifiable, e.g. Starbucks, McDonalds, Marlboro, etc.

2018 CA Trash Data Drive
- Website: https://sites.google.com/sfei.org/trash/notes-from-the-field/data-dive
- GitHub Repo: https://github.com/SCCWRP/2018TrashDataDive

Nerd out with Drew direct link: https://sites.google.com/sfei.org/trash/notes-from-the-field/data-dive#h.p_XBOHXHWED_pL

California Trash Monitoring Methods Project: https://sites.google.com/sfei.org/trash/
