# Module Three Data Study Lite

### By Bao-Nhi Vu and Lama Abed

## Overview
Design studies are intensive, longitudinal, collaborative design activities. While they're a powerful tool in your visualization development toolkit, they also take a bit more energy than is reasonable for a module-sized assignment :-) To get you some practice with the design study methodology, you'll conduct a miniature design study with yourselves as both the designer and stakeholder. Your goal will be to design a visualization tool to support the following scenario: 

The US Department of Energy is conducting a review of historical data to try to inform next generation energy policies. They've hired your team to design a visualization tool for exploring their data to understand past patterns in the energy sector and generate data-driven policy recommendations. These recommendations can occur at the federal or state level and can consider information/data beyond that compiled in the provided dataset. The tool should support both exploration and communication for presentations to policy makers (in other words, they should be able to explore the tool and capture screenshots for inclusion in presentations justifying their policy recommendations).

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/On0xL5EX)


## Serving the Project

This piece is an independent webpage served through a local host. Download the HTML and CSS file and run the command: python -m http.server to serve the page. Open the link http://[::]:8000/ and navigate to the HTML file to read the webpage.

## Design Study Process
_Learning:_ The US Department of Energy is conducting a review of historical data to try to inform next-generation energy policies. As a result, our team has been hired to design a visualization tool to explore the data they provided to give light to past patterns in the energy sector in addition to generating data-driven policy recommendations. The goal of the visualization is to act as a tool for policymakers to use as a resource for communication and presentation. The specific target problem that we will focus on is renewable energy adoption patterns and policies at the state level and see what kind of impact that would lead to. It is important because seeing the impact of adapting renewable energy adoption can steer the new generation of consumers into using these resources. When people see how things are changing for the better, adapting renewable energy would gain popularity and would lead to more of a positive impact on the energy industry as a whole. Additionally, promoting the adoption of renewable energy would have a positive impact on the environment by reducing air pollution. The benefit for the economy is that with more instances of renewable energy, the US will be less dependent on imports from other countries and will become more self-sufficient.

_Winnowing:_ The data that will be used to explore the problem is the data set provided by the US Department of Energy on the energy distribution at the state level. More specifically, we will be exploring the energy consumption at the state level from the years 1969-2019 and the types of energy to be explored are the commercial consumption of coal, distillate fuel oil, geothermal, hydropower, kerosene, petroleum, natural gas, solar, wind, and wood. 
The potential bias that it would have is that because the data is measuring commercial energy use, some companies may be downplaying the amount of energy they use when reporting it. This is especially true if they were reporting for the categories of non-renewable energy. Additionally, the entire list of entities that are classified as commercial in the data collection is not disclosed. Therefore, there may be some commercial entities that are not considered because of a technicality. Additionally, the first pieces of data are from the 1960’s. Therefore, there may be some inaccuracies in how the data was collected then compared to how it is collected now. Despite these biases, we want to use data from commercial consumption because large businesses, corporations, and enterprises are the ones who would be using energy on a large scale basis, rather than the use of an individual person. The dimensions of the data that we will be using are necessary and sufficient to support our approach because data over the last 50 years is a sufficient amount of time to shed light on the pattern of energy usage by state. Additionally, the types of energy are chosen because they represent a wide array of energy that is considered renewable and nonrenewable. 

_Discover:_ The first task that we will want to conduct with the data is showing a state’s commercial consumption of nonrenewable energy so that users can identify patterns in use and year. Why? because we want to show the progression over time of the commercial use of different energy sources. How this is conducted is by showing the British thermal units of renewable and nonrenewable sources of energy by state in an easily comparable way. What the task seeks to learn is showing a wide range of data over a large time frame, an accurate pattern can be seen and assumptions may be drawn from them. Where the task operates is in the space of the years 1969-2019 in the realm of commercial energy consumption. When the task is performed is as part of data exploration prior to hypothesis formation. Finally, who is executing the task is policymakers working for the US Department of Energy.
The second task that we will conduct is to show the pattern of renewable energy usage over those years. Why? because we want to show how some types of energy usage may be popular and widely available in some states but not others. How it is conducted is by showing the geographical location of states and displaying their commercial energy consumption. What this task seeks to learn about the data is the geographical factors that relate to commercial energy consumption. Where the task operates is in the commercial energy consumption by state. When the task is performed is as part of the data exploration process prior to hypothesis formation. Who is executing the task is policy makers working for the US Department of Energy. 

_Design:_ This low-fidelity prototype was designed with the intention to be easy to use so that there was not a high learning curve when using the product. To emphasize this ease of use, there is an “Instructions on Use” panel included in the visualization. Additionally, if we were to include all the data on the screen for 50 US countries, it would be information overload. Therefore a “Filters” panel is on the left where users can choose the state to view, which source of energy they want to focus on, and if they want to see renewable or nonrenewable energy.
The trade-off of the design is that because the visualization is so easy to use, the “Instructions on Use” panel may not be completely necessary and would be an eye-sore if users were to take a screenshot of this entire visualization for presentation. Additionally, with so many countries in the United States, the “Filters” panel may be hard to navigate in addition to the other filters when the panel is long and narrow. This may make the energy source section of the filters unnecessary. Another trade-off is the first graph. The first graph allows the user to see one state at a time. However, this is information overload because there are 50 US states to choose from. Finally, the title of the visualization is located at the bottom, which is unconventional and was placed there because a panel in that location best fits the sectioning of the visualization. However, it may be confusing for users who are using this visualization because of its low learning curve. 

_Implement:_ This solution was implemented using the D3 framework and is a standalone website. The final elements were included in the implementation of the visualization because we wanted the visualization to be self-explanatory so that someone, such as policymakers who may have less technological experience, may be able to use our visualization with a little to no learning curve. The research on the problem space and formative investigations include finding similar and related visualizations that compared sectors of energy consumption by state. In our research, we noticed that many comparisons look at an overarching picture and do not visualize the data, especially from a geographical point of view. So, our visualization took an unconventional approach to visualize the data in an effort to reveal a new perspective for comparing data to help express different conclusions. In particular, the diversity of how each state adapted to different sources of energy can lead users to question and investigate for reasons as to why each state followed a personalized path in energy consumption, whether renewable or nonrenewable 

_Deploy:_ The tasks that we outlined in step 3 are showing a state’s commercial consumption of nonrenewable over the course of 50 years from 1969 to 2019 and showing the pattern of renewable energy usage over those years. The observations about the data that we gained through these tasks is that over the course of 50 years, none of the states in the US use renewable energy sources as their main mode of commercial energy consumption. In fact, it is rare that a state commercially consumes renewable energy sources at all. Recent exceptions to this are states along the East Coast, who are seen to use more solar power compared to other regions in the US. Additionally, across the entire country, the main sources of energy come from distillate fuel oil, petroleum, and gas. States such as New York actually use the most petroleum of all time out of all 50 states in 50 years. However, New York consumed petroleum the most in 1969 and gradually lowered their consumption to match the values of other states. 

_Iterate:_ A new task that we would conduct now that we’ve had a chance to investigate the dataset is to display the different geographical regions of the US. Why this task is pursued is to further explore the geographical location of states in relation to their popular types of commercial energy consumption. How this task is conducted is by separating the US into the west, midwest, northeast, and south regions in their own separate panels. What this task seeks to learn about the data is the geographical factors that push the popularity of the specific consumption of commercial energy sources. Where the task operates is across all states and 50 years of their commercial energy consumption. When the task is performed is as part of the data exploration prior to hypothesis formation. Who is executing the tasks is policymakers under the US Department of Energy. The solution would change to accommodate the task by having 5 panels going horizontally underneath the main map that are smaller. They would display the same information as the main map but be separated by geographical region. 

_Reflect, Pt 1:_ What the solution tells us about the target problem is that geographical regions do play a role in the distribution of commercial energy consumption in each state. Not only in regard to which energy sources are consumed the most but also how distributed energy consumption is to renewable energy sources. The recommendations that we can provide on future policy directions is that the use of renewable energy sources is still a widely untapped resource across all states of the US. By examining the growing use of sources in geographical regions, then the US as a whole can rely less on external imports and invest in itself for energy. The historical patterns that support this recommendation is New York’s use of petroleum had decreased from 1969 to 2019 and it has instead invested in geothermal, hydro, solar, and wind power.

_Reflect, Pt 2:_ What the solution tells us about designing visualizations for the target problem is that understanding the needs of the audience is crucial. For example, when looking into our target problem, we noticed that a lot of solutions did not visualize the states in a map. It was most common to instead display the information in a table, which made it difficult to compare data. So, our solution targeted a specific need by showing the geographical location of states so that it was easier to understand the popularity in their commercial energy consumption. Another aspect was that we needed to create a visualization that was simple and easy to understand. In our initial sketch, we want to have a filter for each state and more filters for renewable and nonrenewable energy. However, if we were to implement this design and distribute it, we would notice that the visualization was less understandable because there were a lot of elements to look at. Therefore, it was hard to get started on drawing initial conclusions with such a detailed approach. 

## Extra Credit
_Live Deployment:_ [Link](https://visdesignstudies.github.io/module-three-design-study-lite-baonhivu/) 
