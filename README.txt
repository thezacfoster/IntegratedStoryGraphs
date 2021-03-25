----------------------------------------------------
     University of Kentucky CS 395-004 Midterm
      Story Graph Traversal Report and README
                  March 25th, 2021

 Made by Evan Shepherd, Zac Foster, and Alex Dingus
----------------------------------------------------

NOTE: 	ALL FILES ARE NECCESSARY FOR RUNNING ANY PRIMARY FILES.
	ALL FILES CAN BE FOUND IN A .zip ON GOOGLE DRIVE AT 
	https://drive.google.com/drive/folders/1MOS3QzfPOWvPS6LtLihYgHv7iWg-YQpz?usp=sharing
	PLEASE UNZIP ALL FILES IN THE SAME FOLDER TO AVOID PATHING 
	ERRORs.

	MUST HAVE CAMELOT INSTALLED TO RUN 
	CS395StoryGraphs.exe OR 
	IntegratedStoryGraph.exe

---------------------------------------------------------------------------------------------------

PRIMARY FILES:

	- TextBasedTraversal.exe
		A command line version of the story graph, used to debug and check 
		specific states and values. Thecurrent version only functions up to
		State 60 due to offset issues in the indexing system, however the 
		graph traversal for the Midterm Stories is 100% possible. In
		addition, while the Player cannot lose below State 60, they can win,
		and an example of a Win path is presented below. To operate,
		simply choose an action from the available list generated for
		each state.
			WIN PATH FROM STATE 0: 277 -> 279 -> 64 -> 281 -> 278

	- CS395StoryGraphs.exe
		A Camelot Project that showcases Midterm Story 1. Has all environments
		built to specification, and includes diversity in the cast present in
		the story. This includes the characters Player, Bandit, Merchant, and
		Guard, the locations Cottage, Crossroads, Market, and Camp, and the 
		environment items BanditChest and Player Coin. This file and it's 
		dependents must be run from Windows Powershell. The instructions are
		provided below.
			1. Open a PowerShell window in the folder of your Camelot executable file.
			2. Using the file path of your experience manager's executable file, run 
			the command "./Camelot.exe -em_path ".../CS395StoryGraphs.exe""

	- IntegratedStoryGraph.exe
		A Camelot Project that attempts to integrate the story graph traversal 
		from file main.cpp with the designed Camelot Environment CS395StoryGraphs.exe. 
		Currently, the Experience Manager only manages a small amount of functionality
		(moving between locations), however it is running simultaneously with the story
		graph for all walk(Player...) actions.
			1. Open a PowerShell window in the folder of your Camelot executable file.
			2. Using the file path of your experience manager's executable file, run 
			the command "./Camelot.exe -em_path ".../IntegratedStoryGraph.exe""

---------------------------------------------------------------------------------------------------

DEPENDENT FILES (ENSURE ALL FILES ARE IN THE SAME FOLDER TO AVOID PATHING ERRORS):

	binary_pruned_states.bin
	binary_pruned_temporal8byte.bin
	pruned_actions.txt
	pruned_fluents.txt
	pruned_values.txt
	pruned_states.csv
	pruned_temporal.csv
	temporal_index.csv
	functions.cpp
	functions.h
