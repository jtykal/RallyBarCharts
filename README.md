# RallyBarCharts
Various old school bar charts - Productivity, Utilization, Story count/points, Task actual hours - per Iteration

jt-ProductivityChart.html
This is a customized version of the Productivity Chart app that appears in the Rally app catalog. It computes team-level Productivity (Points/Hour) using PlanEstimate for points divided by Capacity Hours (from Team Status) for each of the last X (default 10) Iterations (number of iterations is configurable in the app code by setting the "MAX_ITERATIONS" value). It ignores capacity hours for deleted/disabled users. It works only for Teams at the lowest level of the Project Picker -- it does not "roll-up" capacity total from sub-teams (although I am working on this as an update...)

jt-UtilizationChart.html
This is a customized version of the Utilization Chart app that appears in the Rally app catalog. It computes team-level Utilization (Task Actuals/Capacity) for each of the last X (default 10) Iterations (number of iterations is configurable in the app code by setting the "MAX_ITERATIONS" value). It ignores capacity hours for deleted/disabled users. It works only for Teams at the lowest level of the Project Picker -- it does not "roll-up" capacity total from sub-teams (although I am working on this as an update...)

jt-UserStoriesPerIteration.html
This is similar to a Velocity Chart, but has the same look/feel as the other apps in this repository. It displays a bar chart showing either Story Count or Story Points (based on PlanEstimate) per Iteration. It can be filtered by a custom field (LineofBusiness) in the "LOB" value and a Task type (identified by a substring) in the "NAME_MATCH" value. Leave these values empty to include all Tasks. You can also specify the number of Iterations to include in the chart using the "MAX_ITERATIONS" value. This app CAN be used at the team-of-teams level in the Project Picker.

jt-TaskActualsPerIteration.html
This is a bar chart showing a total of Task Actuals (hours) for each Iteration. It can be filtered by a custom field (LineofBusiness) by entering the correct name for the "LOB" constant in the code. Leave this value empty to include all Tasks. Story Count or Story Points is specified in the "ESTIMATION_UNIT" value ("Count" or "Points"). You can also specify the number of Iterations to include in the chart using the "MAX_ITERATIONS" value. This app CAN be used at the team-of-teams level in the Project Picker.
