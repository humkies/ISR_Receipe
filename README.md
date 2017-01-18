# ISR_Receipe

Basic procedure is explained here.

https://indico.cern.ch/event/592621/contributions/2398559/attachments/1383909/2105089/16-12-05_ana_manuelf_isr.pdf


To work with receipe you need two root files

ISRWeight.root file and ISR jets distribution of corresponding sample
you are looking for.

ISRWeights.root and isrjets distribution for few samples are already produced they are here

https://github.com/susy2015/SusyAnaTools/tree/master/Tools/ISR_Root_Files

or you can create your own by using "ISRJetsProducer.C" file. this code works with our regular workflow.

example Makefile is also here.


Everything is done in ISRCorrector.h/cc file and ISRCorrections (up down and central ) are registered to ntuples


https://github.com/susy2015/SusyAnaTools/blob/master/Tools/ISRCorrector.cc#L75-L81


example use is at 

https://github.com/susy2015/HadronicTau/blob/Moriond2017/Tool/CS.cc#L139-L156
 

https://github.com/susy2015/SusyAnaTools/blob/master/Tools/ISRCorrector.cc#L75-L81


If your working directory is different that SusyAnaTools/Tools

Make sure root files are in proper locations and softlinked to your working directory








