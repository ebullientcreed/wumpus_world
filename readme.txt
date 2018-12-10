Name - Navaneeth Thekkumpat

UTA ID - 1001656413

Programming Language used: Java

How the code is structured.
			-Programmed in Java.
			-Sample code is used.
			-In CheckTrueFalse.java added the following functions
			1)tt_entails()	- The method that return if the knowledge base entails alpha .The check is done for kb and 						negation of alpha
			2)tt_check_all()- The symbols in the set are assigned values recursively for each model and once all the symbols 					are assigned value, PL_TRUE() is checked for kb and model. If true then PL_TRUE() is checked for 					alpha and model and result is returned. If the Kb,model is false then return true.
			3)EXTEND()	- Method to extend the model by assigning the passed boolean value to the symbol
			4)PL_TRUE()	- Here the symbols and connectives are evaluated on the basis of different connectives. The 						logic for each connective returns different values for each subexpressions. 
			5)createResult()- Finally the result after checking both the entailment(kb,alpha) and(kb,not(alpha)) is copied 						to the	result.txt. 
			-In LogicalExpression.java modified 
			1)setUniqueSymbol()-The hashset unqset and negunqset is used to extract all the uniquesymbols present while 						reading kb and alpha.

Files		   :	-Submited a ZIPPED directory called assignment7_nxt6413.zip in the blackboard. 
			-This zip directory includes CheckTrueFalse.java, LogicalExpression.java, wumpus_rules.txt and readme.txt files.
			-Keep all input files in the same directory.
How to run the code: 	1)Compile the both CheckTrueFalse.java and LogicalExpression.java the following command
				javac CheckTrueFalse.java 
				javac LogicalExpression.java 
		    	2)Run using the following command 
				java CheckTrueFalse wumpus_rules.txt [additional_knowledge_file] [statement_file]
				Eg:
				- java CheckTrueFalse wumpus_rules.txt b.txt c.txt
			

References	   : 	1) The tutorial on tt-entails- http://vlm1.uta.edu/~athitsos/courses/cse4308_fall2016/lectures/03a_tt_entails.pdf 
			2) Referred https://www.geeksforgeeks.org/hashset-in-java/ - working of hashset
			3) Artificial Intelligence A modern Approach Second Edition by Russel, Norvig			
			4)Scaffolding code provided by author james spargo.
			
			




