# VISUM Format
The output contains the following files to describe the solution:
-	Skim.mtx: text file with skim data for 
-	Netfile.net: text file with link loads for different assignment methods and public transport supply data 
-	Versionfile.ver: binary demand and supply data in VISUM Format 		
-	ProcedureSequence.xml: list of calculation steps.

## skim.mtx 
-	in-vehicle time
-	walk time	
-	transfer waiting time	
-	number of transfers
-	perceived journey time

## netfile for links and public transport supply
### network_solution_assignmentmethod.net
	-	links
### network_solution_put_supply.net
-	lines
-	lineroutes
-	linerouteitems
-	timeprofiles
-	timeprofileItems
-	vehiclejourneys
-	vehiclejourneyitems

## ProcedureSequence.xml
Further explanations are provided in each procedre sequence file. The following procedure sequences are provided mainly for different public transport assignment settings: 
-	VISUM17_PuTAssignment_CapacityRestrictionNo_LineBlockingInterliningYes_v01.00.xml
-	VISUM17_PuTAssignment_CapacityRestrictionYes_TI_10min_v01.00.xml
-	VISUM17_PuTAssignment_CapacityRestrictionYes_TI_01min_v01.00.xml
