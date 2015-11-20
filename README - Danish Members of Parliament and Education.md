
#GENERAL
In this repository you will find a script for R v. 3.2.2 that will recreate some basic elements in Mikkel Torp Thomsen's and my 
study of educational affiliations between of parliament per 4th of december 2014. 

You can find a short description of the study in the links below:
http://www.politiko.dk/perspektiv/politikerfabrikken (Danish)
http://golovchenko.github.io/projects.html (English) 

The data set is ment for practice for those of you who want to learn how to do similar projects. Making the script work means that you
can easily do Social network Analysis in R on your own. 

Please note that the script does represent the entire study. Working with such data requires an enormous amount of choices which are not
possible to document shortly. Please contact me, if you are interested in specific details.

#DATA COLLECTION
The data has been collected from folketinget.dk from the publicly available CV section for each MP. Due to the messy nature of the site,
the entire data set was gathered manually. 

We have registered the educational institutions and start/end date for each education. In cases where only the end date was provided,
we assumed that the politician studies bachelor and masters for 6 years in total. 

In the Analysis we only focus on 8 most represented educational categories in the parliament. This means that we only analyze 117 Members
of Parliament out of 179. 

# WHAT ARE THE CONNECTIONS? 
A connection between two members means that they have officially been students at the same institution during one year, for instance at
the Department of Economics at Copenhagen University in 2013. This does not necessarily mean that they have been physically copresent
at the same department simultaneously. This will not be the case if politician A graduates in the first half of 2013 while politician B 
enters the department during the second half of 2013. In both cases they have a connection in the graph because they study at the same 
place during the same year – but not simultaneously. Another important example would be if the politicians are officially enrolled at 
the department but are not active during a specific period (due to an exchange program, maternity leave etc.). The chances of person A 
and B of meeting each other, however, increase the more years they are enrolled in the same institution
