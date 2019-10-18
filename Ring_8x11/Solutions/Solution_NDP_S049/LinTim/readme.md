# LinTim Format

All LinTim input files can be opened with a text editor.

The input contains the following folders to describe the network supply and solution:

-	basis
- 	delay-management
- 	line-planning
- 	timetabling
- 	vehicle-scheduling

For more information on the folders and their contents, have a look at the [LinTim documentation](https://gitlab.gwdg.de/LinTim/OpenLinTim/blob/master/doc/documentation.pdf).

Additional the following files are given to characterize the solution:

- 	Description.csv: Containing a small description on the specific dataset, i.e., the method used for creation
- 	Kenngrößen: Evaluation parameters calculated by LinTim
- 	perceived_travel_time_output.tim: The demand and perceived travel time for each od pair