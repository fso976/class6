
# class-hw5
CEBD1160 Homework #5 
Assignment 5 - Psuedocode

A) loading dataset 

Initialize all relevant libraries
Initialize importing dataset to path
If filename found 
	Print success
Else
	Print failed
Endif

Load dataset into dataframe
	Set flag to filename
	Set flag Seperator to trailing whitespaces 
  Set flag Header to True
	Set flag engine to Python

B) organize

Remove header and/or index if any exists
If row[0] in file holds int or float && col[0] is not an index
	break
	If col[0] is index && row[0] is String
		Set flag to newfilename
		Set index to False
		Writing to a new csv file
  Else 
	  Set flag to newfilename
	  Set header to True
    Set index to False		
    Writing to a new csv file
Endif

transpose the data
read from newfilename

C) compute summary statistics

Calculate average for one column
set sum to 0
set avg to 0
for elemt in index
	sum += elemt
return sum

avg = sum /  length of index

D) Visualize the data, 1-feature (column) at a time, i.e. histogram, and save the figures to files 

Import matplotlib 

set x = dataset
for i, col in enumerate(index):  
run hist method
	set flag x = dataset([i-1:i])
  set bins size
  set xlabel
  set ylabel
  set title 
  show plot 
  Save figure to file

E) Visualize the data, 2-features (columns) at a time, i.e. scatter plot, and save the figures to files,

Import matplotlib 

Set seed = N 
set x, y = dataset

for row1 in index:
	row1 = row[index]
	for row2 in index: 
    y = row[index+1]
    run scatter method on row1 and row2
	  set flag x for dataset

  plot([‘row1’], [‘row2’])
  set xlabel
  set ylabel	
  set color for each colmn
  set title 

  show scatter plot 
  Save figure to file

2. (intermediate) 

F) Pseudocode for adding header data to your table, for an arbitrary one of these datasets,

for row in index:
	row[index] = row[index + 1]
 Add a list of header at row[0] start at col[1]

3. (reach) 

G) Pseudocode for an additional type of plot (Google to find plot types of interest) for visualizing 2 or more of the features at a time.
Recommendation: plan to use `matplotlib` for plotting






























=======
# class6
>>>>>>> bf571afdf37432a09f8cd55d71244a69764a6605
