This repository provides a comprehensive set of DAX equations for building a quality dashboard. The dashboard includes metrics for tracking defects.

Three data tables are used in this dashboard, connected through relationships. The DAX formulas utilized are:

![image](https://github.com/srashmii/Quality-Dashboard/assets/152070309/1b4f58c4-59aa-4019-acd9-6fc49268c6c6)


1.**Defect%** = DIVIDE(SUM('Quality Data'[Defects]),SUM('Quality Data'[Samples]),BLANK()) 

2.**Fatal error%** = DIVIDE(SUM('Quality Data'[Fatel Errors]),SUM('Quality Data'[Samples]),BLANK()) 

3.**Quality Score** = IF([Defect%]=blank(),BLANK(), 1-[Defect%])

4.**Sampling%** = DIVIDE(SUM('Quality Data'[Samples]),SUM('Quality Data'[Total Task]),BLANK())

![image](https://github.com/srashmii/Quality-Dashboard/assets/152070309/2fa94d2b-b36f-4d93-8792-9320ffc637b0)
