# Regions sanitàries (RS), Sectors Sanitaris (SS), Àrees de Gestió Assistencial (AGA) i Àrees Bàsiques de Salut (ABS) de Catalunya

Fitxers GeoJSON de les regions sanitàries, sectors sanitaris i àrees bàsiques de salut de Catalunya a punt per ser representats en mapes webs sota llicència [GNU AGPLv3](https://choosealicense.com/licenses/).

Agraïr la [versió original](https://salutweb.gencat.cat/ca/el_departament/estadistiques_sanitaries/cartografia/) d'aquestes dades cartogràfiques a la Generalitat de Catalunya - Departament de Salut - Direcció General de Planificació en Salut. Més informació en el fitxer `Catàleg de metadata.pdf`

Les dades han estat convertides per la Glòria Macià de format `shapefile` (`.shp1`) a format GeoJSON fent servir [QGIS](https://www.qgis.org/ca/site/), un sistema d'informació geogràfic gratuit i de codi obert, fent servir CRS 4326 pensat per a mapes web. 


## Les regions sanitàries

Les [regions sanitàries](https://catsalut.gencat.cat/ca/coneix-catsalut/catsalut-territori/regions-sanitaries/) són demarcacions territorials basades en el principi de descentralització del sistema sanitari públic, que té com a objectiu l'apropament i l'accessibilitat dels serveis a tota la població.

Aquestes regions estan delimitades atenent factors geogràfics, socioeconòmics, demogràfics, laborals, epidemiològics, culturals, climàtics, de vies de comunicació homogènies, així com d'instal·lacions sanitàries existents, tot tenint en compte l'ordenació territorial de Catalunya.

Compten amb una dotació adequada de recursos sanitaris d'atenció primària i d'atenció especialitzada per atendre les necessitats de la població. Cada regió s'ordena, al seu torn, en sectors sanitaris.

![image](https://user-images.githubusercontent.com/17580456/147409628-729c0225-0f68-4b54-b435-eba3f5b2bd3a.png)


## Els sectors sanitaris
Els [sectors sanitaris](https://catsalut.gencat.cat/ca/coneix-catsalut/catsalut-territori/regions-sanitaries/) són l'àmbit on es desenvolupen i coordinen les activitats de promoció de la salut, prevenció de la malaltia, salut pública i assistència sociosanitària en el nivell d'atenció primària i de les especialitats mèdiques. Els sectors sanitaris estan constituïts per l'agrupació d'àrees bàsiques de salut.

![image](https://user-images.githubusercontent.com/17580456/147409637-41c3e13a-a8fe-464f-a8b3-ce2b9d4c49a1.png)

Els [sectors sanitaris](https://catsalut.gencat.cat/ca/coneix-catsalut/catsalut-territori/regions-sanitaries/) són l'àmbit on es desenvolupen i coordinen les activitats de promoció de la salut, prevenció de la malaltia, salut pública i assistència sociosanitària en el nivell d'atenció primària i de les especialitats mèdiques. Els sectors sanitaris estan constituïts per l'agrupació d'àrees bàsiques de salut.

## Àrees de gestió assistencial 
[Les àrees de gestió assistencial](https://catsalut.gencat.cat/ca/proveidors-professionals/registres-catalegs/catalegs/territorials-unitats-proveidores/) (AGA) són delimitacions territorials que parteixen de l’agrupació d’àrees bàsiques de salut (ABS). Aquesta delimitació correspon a criteris de planificació operativa, de coordinació i d’anàlisi dels fluxos principals entre l’atenció primària i l’hospitalària bàsica.

![image](https://user-images.githubusercontent.com/17580456/147409612-df6c89ac-8182-4d35-b62c-01ede2e4aff4.png)


## L'àrea bàsica de Salut
[L'àrea bàsica de salut](https://catsalut.gencat.cat/ca/coneix-catsalut/catsalut-territori/regions-sanitaries/) (ABS) és la unitat territorial elemental a través de la qual s'organitzen els serveis d'atenció primària de salut. Són unes unitats territorials formades per barris o districtes a les àrees urbanes, o per un o més municipis en l'àmbit rural.

![image](https://user-images.githubusercontent.com/17580456/147409510-c76b3b12-44cf-4f6f-909b-99c67a53186d.png)

## Mapa Web 

La carpeta `mapa-web` conté el codi necessari per reproduir un mapa web similar a aquest. Tot i que estrictament forma part d'un altre projecte sobre com la ciència de dades pot col.laborar a reduir la desigualtat en l'accés a especialistes per malalts de Malaltia Inflamatòria Intestinal (MII), es presenta de manera conjunta en un repositori com a exemple d'ús dels polígons GeoJSON. 

![image](https://user-images.githubusercontent.com/17580456/147416503-c5d1febb-6830-4779-8584-860d1b239771.png)

## Desigualtat d'accés a especialistes entre els malalts de MII a Catalunya
### Un estudi d'Enginyeria i Ciència de Dades

Es crea una base de dades `mii/hospitals` a partir de l'informació de Catsalut sobre els [centres del SISCAT](https://catsalut.gencat.cat/ca/centres-sanitaris/cercador/) que presten serveis segons siguin d'atenció primària (CAP, alguns d'ells amb atenció continuada, i consultoris locals) i els centres d'atenció especialitzada (hospitals, centres sociosanitaris i centres d'atenció a la salut mental). S'escullen els hospitals i s'enriqueix la informació amb la geolocalització de l'hospital, el codi de la regió sanitària i la classificació de l'hospital segons el [`delphi consensus statement`](http://www.scdigestologia.org/docs/plans_estrategics/pla_estrategic_MII_2020.pdf) disponible a la web de la [Societat Catalana de Digestologia](http://www.scdigestologia.org/docs/plans_estrategics/mii/Directori_unitats_MII.pdf). 


