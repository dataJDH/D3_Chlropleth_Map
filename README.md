# D3_Chlropleth_Map
Map with number of earthquakes per state with mouseover effect

Provided datasets:

`state-earthquakes.csv`: each record represents a state and is of the form <State,Region,2010,2011,2012,2013,2014,2015,Total Earthquakes>, where
`State`: the name of the state. e.g., Alabama.
`Region`: the region which the state belongs to. e.g., South.
`2010,…,2015`: the number of earthquakes in that state in 2010, …, 2015, respectively.
`Total Earthquakes`: the total number of earthquakes in that state during 2010-2015 (the number of earthquakes in the state-earthquakes.csv file have been slightly modified from the original values and do not represent the official figures).

`states-10m.json`: A TopoJSON topology containing two geometry collections: `states`, and `nation`. 
 
 A choropleth map where color of each state corresponds to the log of total earthquakes in that state (Total Earthquakes field in state-earthquakes.csv.). i.e., darker colors correspond to higher total earthquakes in that state and lighter colors correspond to lower total earthquakes in that state in log scale. The `states-10m.json` is used to draw the choropleth map. 
A vertical legend shows how colors map to the total number of earthquakes. A tooltip is created using the d3-tip.min library in the lib folder. On hovering over a state, the tooltip shows the following information on each line: (1) state name, (2) region, and (3) total earthquakes. The tooltip appears when the mouse hovers over the state. On mouseout, the tooltip disappears. 

The D3 library is provided in the lib folder.
