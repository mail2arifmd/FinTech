# FinTech
The solution contains following Projects (built on .Net Framework 4.7.2)

A)Core Flagship Product
	1) FinTechBanking.UI
	2) FinTech.Core.Interface
	3) FinTech.Core.DataAccess
B) Product Extension - New Interest Calculation basis balance
	1)FinTech.Client2.Extension
	2)FinTech.Client2.Extension.Interface
C) UnitTest
	1) FinTechBanking.Test


The approach taken here takes into consideration that the Flagship product & its classes are Closed for Modification but open for extension, thus minimising changes to Core Projects

For the Bands with Balance & their Interest Rates, it is best to store these in database & built Strategy Pattern, such that we are not mixing data and behaviour within our code. As such the code is fully maintainable if such bands & their interest slabs change in future

This project hooks an extension to an existing WPF Application, but we can also develop an API that uses the same extension projects to give back response with same interest calculation.

Finally the unit test project is based on MS unitest project template & contains some sample test cases to test the Interest calculations

Due to time constraints, could not code exception handling.

Please let me know if you have any queries or need further explanation
