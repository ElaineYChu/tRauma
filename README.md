# tRauma: A dynamic database of blunt rib trauma
This repository contains screenshots of a Shiny application developed using the doctoral dissertation data of 
>**Dr. Cortney N. Hulse** and funded through a National Institute of Justice Graduate Research Fellowship (Award [2019-R2-Cx-0047](https://nij.ojp.gov/funding/awards/2019-r2-cx-0047)). 

All code, functions, and design were executed by Elaine Y. Chu, with UX input provided by Briana T. New, Kyra E. Stull, and Christopher A. Wolfe.

## Screenshots

### Reference Data Tab
![](/screenshots/new_main_tab.png)
This tab allows the user to dynamically edit 1400+ reference cases for certain demographic information using the *Edit Data* drop-down tab, such as:
* Age  
* Sex  
* Height  
* Manner of Death
* Cause of Death
* Certain Rib Numbers or Side
* Rib Trauma Location

Changes to the reference data are then reflected in the *Heat Map* and *Reference Data Summary* drop-down tabs. 

The *Heat Map* provides a visual summary of all document trauma by 1) Rib Number, 2) Rib Side, and 3) Rib location, where: 
* a = anterior
* al = antero-lateral
* pl = postero-lateral
* p = posterior

### Search by Fracture Location Tab
This tab allows for the user to input blunt trauma locations and returns all matching reference cases using a recommender-system-like approach. The similarity metric *sim_idx* provides the degree of similarity of a reference case to the user-input on a scale of least similar (0) to most similar (1). The page is separated into three (3) sections: 

#### Rib Diagram
![](/screenshots/new_fracture_tab_rib-diagram.png)

Using the rib diagram, a user can input case-specific rib trauma by drawing a box around trauma locations. Each trauma is added individually, using the *Add Trauma Location* button. The *Check your input* space above the diagram is for the user to keep track of already-added locations.

#### Matching Reference Cases
![](/screenshots/new_fracture_tab_matching-cases.png)

All cases within the similarity index range provided by the user will be displayed, in descending order from most-similar to least-similar. All reference columns selected in the **Reference Data Tab** will be included for each case. 

#### Descriptive Statistics
![](/screenshots/new_fracture_tab_descriptive-stats.png)

This section allows for the user to evaluate the counts and density of demographic information for the matching reference cases. Either a bar chart or density plot is provided based on the category defined by the user in the drop-down menu.


