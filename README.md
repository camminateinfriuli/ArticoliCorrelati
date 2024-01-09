# ArticoliCorrelati
 ArticoliCorrelati è una modifica di related_items per una diversa acquisizione dei correlati, in particolare ricerca prima gli articoli che hanno la stessa metakey e poi in mancanza di risultati esegue l'acquisizione nel metodo normale, cioè utilizzzando una corrispondenza anche parziale.
 
 Esempio: metodo modificato da risultato solo con corrispondenza esatta
 
 metakey            SI             testo ricerca        NO
 "pera"             -->          "pera"                 -->         "peraltro"
 "alto fragile"     -->          "alto fragile"         -->         "alto","fragile" 

 Esempio: metodo normale da risultato anche con presenza parziale nel testo di ricerca
 metakey            SI             testo ricerca        SI
 "pera"             -->          "pera"                 -->         "peraltro"
 "alto fragile"     -->          "alto fragile"         -->         "alto","fragile"  

 Se la ricerca con metodo modificato non da risultato o da risultato inferiore al numero massimo di rispondenze come da impostazioni del modulo vengono elencate prima le rispondenze con metodo modificato e poi le rispondenze con metodo normale fino al raggiungimento del numero massimo impostato.