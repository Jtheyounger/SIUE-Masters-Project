All code was written and run in Spyder 5.4.1 with Python 3.10.9 as the base (utilized through Anaconda)

Runnable code can be found in the folder "Project Code"

For all code, be sure to change the Prefix variable located at the top of every program to the location
you have put the folder. This variable can be found at...

Line 13 for CSVtoGraph.py
Line 13 for ProjectFunctions.py
Line 17 for SongAnalysis.py
Line 19 for SongGeneration.py

To use the generated MIDI feature in SongGeneration.py, be sure to install the library midiutil. If the library
is not installed, just select "no" when asked if you want a MIDI file created

CSVtoGraph.py - Turns csv files created from MIDI files into adjacency matrices

ProjectFunctions.py - Enables sheet music to be written

SongAnalysis.py - Fills out oldTimeNetworkInsights.csv and irishNetworkInsights.csv for data analysis, and creates
		aggregate graphs for A, C, D, and G Major for Irish and Old-Time

SongGeneration.py - Creates new tunes based on selected parameters.
	
	After typing every number for the below, be sure to press "enter" to proceed
	When prompted to generate an Old-Time or Irish tune, type 1 for Old-Time, 2 for Irish
	When prompted to select song's key, type 1 for A Major, 2 for C Major, 3 for D Major, or 4 for G Major
	When prompted how long you would like the section to be in notes, type a number (50 is encouraged)
	When prompted for how far from starting pitch you want to go, type any number (I choose 7 to 10 usually)
		51 will ensure all notes are available for your song, but it may wander all over the place
	When prompted how many song sections you'd like, 2 is the usual number. This is how many different parts 		
 		there will be
	When prompted with how many times to repeat each section, 2 is the usual number. This is how many times
		each unique section will be repeated
	When prompted for bowing method, this will apply to the MIDI file. Press 1 for normal whole notes, or 2
		for a bowing that consists of a whole note followed by 2 half notes, repeated over and over
	When prompted for generating a MIDI file, press 1 for Yes, press 2 for no.
		(Be sure to have midiutil downloaded before pressing 1)

	Your generated tune's sheet music and MIDI file (if chosen) will be created in the Generated Tunes folder


Folder Breakdown

	Aggregate Graph Visualizations - Complex Networks made in Gephi from the aggregate graph adjacency matrices
	Generated Tunes - Where sheet music and midi files will be created from SongGeneration.py
	irish_adjacency_matrices - Where the Irish adjacency matrices are created
	irish_csv_files - Where Irish csv files made from Irish MIDI files are stored
	irish_midi_files - Where downloaded Irish MIDI files are stored
	old_time_adjacency_matrices - Where the Old-Time adjacency matrices are created
	old_time_csv_files - Where Old-Time csv files made from Old-Time MIDI files are stored
	old_time_midi_files - Where downloaded Old-Time MIDI files are stored
	Project Code - Where code for the various parts of the project can be found, along with the master guide
		to the song filenames for various folders, and aggregate graph adjacency matrices
	R Studio Files for Predictions - Where R Studio code and the excel file the code analyzes can be found.
		The spreadsheet in this folder is a combination of irishNetworkInsights.csv and 
		oldTimeNetworkInsights.csv from the Project Code folder
