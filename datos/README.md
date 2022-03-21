# Contenido:
  
- Ppinaster_CyL-datos_ejemplo.xlsx: estructura de inventario de con datos ejemplo para Pinus pinaster en Castilla y León.
- Psilvestris_CyL-datos_ejemplo.xlsx: estructura de inventario de con datos ejemplo para Pinus sylvestris en Castilla y León.
  
Los 2 archivos mencionados anteriormente fueron rellenados con datos de parcelas obtenidas de las distintas calidades de estación propuestas en: [Del Río et al. (2006)](https://medioambiente.jcyl.es/web/jcyl/binarios/566/228/01-GESTION%20FOREST_CORREGIDO2.pdf?blobheader=application%2Fpdf%3Bcharset%3DUTF-8&blobheadername1=Cache-Control&blobheadername2=Expires&blobheadername3=Site&blobheadervalue1=no-store%2Cno-cache%2Cmust-revalidate&blobheadervalue2=0&blobheadervalue3=JCYL_MedioAmbiente&blobnocache=true)  
  
- IFN: carpeta que contiene datos del Inventario Forestal Nacional
	
# Datos ejemplo:
  
En los 2 documentos de ejemplo para Castilla y León encontrarás dos hojas de datos. La hoja "Parcelas" hace referencia a la información de la parcela:  

- INVENTORY_ID: identificador de inventario, puedes poner la fuente de donde has obtenido los datos (OJO, los árboles de la parcela deben llevar el mismo código)
- PLOT_ID: identificador de parcela, en donde debes poner un código numérico (no te líes, sirve con 1, 2, 3...) (OJO, los árboles de la parcela deben llevar el mismo código)
- SPECIE_IFN_ID: es el código de referencia que corresponde a la especie principal de la parcela según el Inventario Forestal Nacional. Puedes consultarlo en la página 24 de este documento: https://www.miteco.gob.es/es/biodiversidad/servicios/banco-datos-naturaleza/documentador_bdcampo_ifn3_tcm30-282240.pdf
- YEAR: año de partida
- AGE: edad promedio de la parcela (años)
- DENSITY: densidad de la parcela (pies/ha)
- BASAL_AREA: área basimétrica de la parcela (m2/ha)
- DOMINANT_H: altura dominante de la parcela (m). Puedes calcularla haciendo el promedio de la altura de los 100 árboles más altos por hectárea (ordena los árboles de mayor a menor altura, y ten en cuenta que cada árbol representa a un nº de árboles determinado a nivel de parcela (factor_expansion); suma el factor de expansión hasta llegar a tener los 100 primeros árboles más altos y haz el siguiente cálculo:  

	              (factor_expansion_1·h_1 + factor_expansion_2·h_2 + ... + factor_expansion_n·h_n)/100  

- MEAN_H: altura promedio de los árboles de la parcela (m)
- QM_DBH: diámetro medio cuadrático (cm)
- VOL: volumen de madera con corteza (m3/ha)
	      
La hoja de "PiesMayores" hace referencia a la información sobre los árboles de la parcela:  
- INVENTORY_ID: el mismo código de la parcela a la que pertenece el árbol  
- PLOT_ID: el mismo código de la parcela a la que pertenece el árbol  
- TREE_ID: identificador numérico único del árbol dentro de la parcela (no te líes, sirve con 1, 2, 3...)  
- expan: es el número de árboles al que representa el árbol sujeto a nivel de hectárea. Se calcula así: (10.000 m2) / (superficie parcela en m2)  
- dbh: diámetro del árbol (cm)  
- height: altura del árbol (m) 
- basal_area: área basimétrica del árbol (cm2)

