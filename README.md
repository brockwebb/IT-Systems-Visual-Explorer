# IT-Systems-Visual-Explorer
This is a visualization using the Open Source D3 Javascript library to explore IT system interfaces. The goal is to make it convenient for a large enterprise to examine the interfaces within the system architecture based on the current configuration. Many tools and features will be added that make the various tasks needed more convenient and help to quickly understand the relationship and data flows between system components. A "toy" system is provided as an example, but will be able to display any system if the data is available and can be put in the right format for ingest.
Legend:

#Motivations for this tool

This is designed to quickly look at all systems together and discern the various data flows between systems. The goal was something visual, easy to use, and would quickly identify the various links that Census systems share. When conducting performance analysis, understanding the consumer/customer relationship between systems is important in a holistic understanding of how systems interact and interoperate.

#Current Tasks
* Clean up the source and provide "in line" references (general references included below)
* Seperate out javascript from the HTML and use includes to clean up the file
* Put a working version on CodePen (Completed 3/1/2016: http://codepen.io/brockwebb/pen/VaYzZw)

#Potential Improvements
* Adding data type labels (e.g. (P) patadata; (R) response data; (S) sample data; etc)
* Identify the type of interface better: ESB, DBLink, SFTP, etc.
* Adding filters for system nodes and data types, by group (area), etc.
* Setting up graph to group like colors together
* Adding a toggle to "turn on" sub-group colors, cluster those together
* Retrieve data dynamically from a JSON or XML document, allowing dynamic creation and push to the display, or a custom select of a file to display
* Data path analysis: help trace data lineage from a source system, across system boundaries and interfaces, to a destination of interest
* Open to suggestions

# Recent Complietions (v0.51b)
* Restructured input into link[] and node[] inputs to get group colors working
* Added a legend.
* Created an Excel File to create and maintain groups and link relationships, cut-n-paste the resulting code into the link[] and node[] variables.

#References
Reference "in line" in the source still need to be cleaned up. Until that time, this is an adaptation of:
* Open Source D3 javascript library
* Mike Bostock's Force Directed Graph
* Simion Raper's adaptations for node neighbor highlighting
* Rom2BE's grouping example http://jsfiddle.net/Rom2BE/H2PkT/
