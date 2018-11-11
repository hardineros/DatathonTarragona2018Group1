# DatathonTarragona2018Group1
Code from Group 1: Data Quality. Tarragona Datathon, November 11 &amp; 12, 2018, Spain. Meassuring eICU data quality: an open and standarized approach.

Our challenge was to create an open, standard and general way to meassure the quality of data from all variables used in the eICU database (2).
 
Introduction:

Although there are many scores that try to measure the same issue, most of them are really specific for one kind of variables, for unique tables, or are commercial products. We took the Data Quality Dimensions (2)  as our base model. Here we have documented all R code used to face our challenge.

We have tested several R packages and have choosen the Data Quality diagnosis (3) to test each variable inside a table. Based on the content in each table we applied different code to adjust for numeric versus categorical variables. Then we have constructed a Table Data Quality Score, meassuring and averaging the missing and outliers score for each variable on each eICU table. Basing on recommendations we propose these cutting points to compare results:

The method proved to be a feasible approach that we believe can be extended to other databases. One of the limitations of this approach was the lack of a well documented database dictionary. This made it difficult to fully understand the meaning of each field and table and which fields accept NULL values. 

This work and common effort could be a starting point to create an International Critical Data Index (ICDI). A more thorough description of the variables commonly found in the tables, documented in a standard way, would support better and wider big data, machine learning and a collaborative investigation framework. This could also improve potential interoperability between other databases. 

Group 1 Members: Teresa Rincon, <tarincon1@gmail.com>, Boston, USA. Juan Alfonso Soler, <jsolerbarnes@gmail.com>, Murcia, ESP. Josep Trenado <jtrenado@mutuaterrassa.es>, Terrassa, ESP. Ariel Leonardo Fernandez <hardineros@hardineros.com>, Buenos Aires, Argentina.s

References:
1. Goldberger AL, Amaral LAN, Glass L, Hausdorff JM, Ivanov PCh, Mark RG, Mietus JE, Moody GB, Peng C-K, Stanley HE. PhysioBank, PhysioToolkit, and PhysioNet: Components of a New Research Resource for Complex Physiologic Signals. Circulation 101(23):e215-e220 [Circulation Electronic Pages; http://circ.ahajournals.org/content/101/23/e215.full]; 2000 (June 13).
2.IBM. Data quality dimensions. IBM. Retrieved November 11, 2018, from: https://www.ibm.com/support/knowledgecenter/en/SSZJPZ_11.5.0/com.ibm.swg.im.iis.ia.product.doc/topics/r_quality_indicators.html
3. Choonghyun Ryu. Data quality diagnosis. Retrieved November 11, 2018, from: 
https://cran.r-project.org/web/packages/dlookr/vignettes/diagonosis.html
