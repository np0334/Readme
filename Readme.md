Create Tree using JSTree

Application to read and display the data using a tree component. User will also be able to add or remove node. The file format for the data being accessed from is ’.csv’.

Getting Started

Prerequisites

You will need a web browser that runs a server in backend like Firefox.

Installing

Copy the compressed folder anywhere on your disk. 
Unzip the folder.
Open the html file “TreeusingJSTree.html” in Firefox (or any similar web browser.).

About the Code 

Files and Description

Scripts

‘treeusingJSTree.js’ includes the script used to run the project.

Function : successFunction
	This function takes the data from the .csv file and converts it into the JSON array. CSV is basically Comma Separated Values, hence ‘,’ is used to separate each value in ‘.csv’ file.
	I created a array of headers which stores the heading of all the columns. I am using the JSTree which accepts JSON in the format of {“id”:” ”, “parent” : “”, “text”: “”}. Therefore, I have written a code to convert ‘parent_id => parent’, and ‘name => text’. 
	Finally, I get the JSON array in arrayJson.

Creating Tree.
	jsTree is jquery plugin, that provides interactive trees. It is absolutely free, open source and distributed under the MIT license. jsTree is easily extendable, themable and configurable, it supports HTML & JSON data sources and AJAX loading.

	By accessing each node the code calculates the amount of the nodes. Please note the amount of the nodes is calculated using the given data.
For example:
The root node is: Kropf with amount 48.67 but the sum of its children is 356.67.



	The two “on click” functions create and delete perform the create node and delete node operations respectively, by using predefined functions in jsTree.

HTML file

	The html file includes the style.min.css, bootstrap.min.css, jquery-3.2.1.min.js, jstree.min.js, treeusingJSTree.js, treeusingJSTree.css.

There are 2 buttons create and delete, to create and delete the node from the tree. 
When a create button is clicked it creates a new node and asks to enter the amount for that node. You can name the node after it is created. You can only create a new node when you select a parent node for that new node.
The Delete button can be used to delete the selected node from the tree. If the selected node is a parent node then it will delete its children along with the selected node.

Authors

Neha Pardeshi