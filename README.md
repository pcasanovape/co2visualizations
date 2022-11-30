# PAC 2 – M 2.959 Visualització de dades
### Estudi de tècniques de visualització de dades


## Autor de la PAC
Activitat realitzada per **Pau Casanova Pedrol**.


## Introducció
Aquest repositori GitHub ha estat creat amb la finalitat de publicar i compartir les visualitzacions realitzades en el marc de la PAC 2 de l'assignatura de Visualització de dades del màster de ciència de dades de la UOC, així com els arxius que s’han utilitzat per a crear-les, des del dataset original fins al codi del preprocessament de les dades i de generació de visualitzacions.


## Dataset escollit
El dataset original s’ha descarregat del repositori GitHub “co2-data” de la pàgina Our World in Data, que analitza diversos aspectes sobre les emissions de CO2 i gasos efecte hivernacle de tots els països del món, amb observacions anuals des de l’any 1750 (en alguns casos) fins a l’any 2021. La pàgina original on es s'ha publicat l'anàlisi realitzada amb aquestes dades es pot veure en el següent enllaç:

https://ourworldindata.org/co2-dataset-sources

Aquest és l’enllaç al repositori GitHub des d’on s’han descarregat les dades:

https://github.com/owid/co2-data

S’ha escollit aquest dataset ja que és prou ampli i complet per oferir les dades necessàries per qualsevol dels tipus de visualitzacions de l’exercici, que poden servir a més a més per a una millor comprensió del problema de la contaminació de l’atmòsfera.


## Descripció de l’exercici
Per aquest exercici s’ha demanat l’anàlisi i la realització de 3 tècniques de visualització diferents:
1-	Ridgelines
2-	Diagrama de dispersió o scatter plot
3-	Sunburst
Per tenir un fil conductor pel que fa a la temàtica de tota la pràctica, les dades originals parteixen d’un únic dataset, però s’han agafat subsets diferents, que s’han considerat els més apropiats per a cadascuna de les visualitzacions a realitzar.


### Visualització 1
La primera tècnica amb la que treballem s’anomena Ridgeline plot, i es tracta d’una superposició de diferents gràfiques d’àrea que permeten comparar l’evolució al llarg del temps o la distribució d’una variable segons diverses categories.
Per a aquesta visualització s’ha escollit comparar l’evolució de l’emissió de CO2 per càpita de les 10 principals economies mundials des de 1960 fins l’any 2020.
Aquesta visualització s’ha realitzat amb l’app Tableau Public i es pot veure en el següent enllaç:

https://public.tableau.com/views/CO21960-2020/CO21960-2020?:language=es-ES&:display_count=n&:origin=viz_share_link

L’arxiu en format .twbx es pot trobar a la carpeta ‘visualitzacions’ d’aquest mateix repositori amb el nom ‘CO2 1960-2020’.


### Visualització 2
Per a la segona visualització hem emprat la tècnica del gràfic de dispersió o scatter plot, que permet comparar dues variables per a detectar possibles patrons en un dataset.
Per aquesta visualització hem decidit comparar les variables de co2 per capita i pib per càpita de tots els països del món, alhora mostrant amb diferents elements de representació (mida i color) el PIB total del país i el continent en que se situa.
Aquesta visualització l’hem realitzat amb la llibreria ggplot de R i es pot trobar en format PNG a la carpeta ‘visualitzacions’ d’aquest mateix repositori, amb el nom ‘scatter plot’. El codi R utilitzat per a la seva realització es pot veure en format HTML a la mateixa carpeta, amb el nom ‘scatter plot R markdown’.


### Visualització 3
Finalment hem treballat la tècnica Sunburst, que és un gràfic de pastís am múltiples nivells, que permet comparar les parts d’un tot, amb diferents nivells de jerarquia. El primer nivell es situa al centre de la circumferència, i els elements derivats de cada nivell es mostren amb sectors d’anelles circumdants exteriors que es corresponen amb el primer. 
En aquest cas hem decidit representar el percentatge d’emissions de co2 de cada continent i de cada país sobre el total mundial. En aquest cas el nivell 1 són els continents, i el nivell 2 correspon als països. 
Aquesta visualització s’ha realitzat amb l’app Tableau Public i es pot veure en el següent enllaç:

https://public.tableau.com/views/CO2bycountry_16697662037910/CO2bycountry?:language=es-ES&:display_count=n&:origin=viz_share_link

L’arxiu en format .twbx es pot trobar a la carpeta ‘visualitzacions’ d’aquest mateix repositori amb el nom ‘CO2 by country’.


## Codi font rellevant
* **source/preprocessat.html**: Arxiu HTML que conté el codi executat a Jupyter Notebook per al preprocessat del dataset original, i la creació dels arxius .csv que corresponen al subset emprat en cada tècnica de visualització.

* **source/preprocessat.ipynb**: Arxiu .ipynb que conté el codi executat a Jupyter Notebook per al preprocessat del dataset original, i la creació dels arxius .csv que corresponen al subset emprat en cada tècnica de visualització.

* **source/pac2vd_pcasanovape.rmd**: Arxiu RMarkdown que conté el codi executat per a la realització del diagrama de dispersió (segona visualització).


