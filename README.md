# Codifica XML/TEI e Named Entity Recognition – *The Discovery of the Large, Rich, and Beautiful Empire of Guiana*

Progetto di **filologia digitale** e **Named Entity Recognition (NER)** sviluppato nell'ambito del *Laboratorio di Filologia Digitale* su porzioni selezionate di *The Discovery of the Large, Rich, and Beautiful Empire of Guiana* (1595) di Sir Walter Ralegh.

## Contesto storico-critico
L'opera intreccia diario di bordo, resoconto geografico, narrazione propagandistica anti-spagnola (*Leyenda Negra*), autopromozione verso la corte di Elisabetta I e il mito di *El Dorado* / *Manoa*[cite: 1, 2, 3].

## Scelte di codifica XML/TEI
* **Struttura del documento:** organizzazione in `<teiHeader>` e `<text>` (`<body>` e `<back>`), con collocazione delle liste di entità nominate nella sezione `<back>` anziché in `<sourceDesc>`[cite: 3].
* **Tag e attributi principali:** impiego di `<persName>`, `<roleName>`, `<orgName>`, `<placeName>`, `<geogName>`, `<eventName>`, `<objectName>`, `<date>` (con `when` e `dur` in formato ISO `P5D`, `P7D`) e `<rs>` con attributi `ref`, `type`, `subtype`, `role` e `xml:lang` (es. per toponimi bilingui come `Point Curiapan` / `Punta de Gallo`)[cite: 3, 4].
* **Liste tassonomiche nel `<back>`:** strutturazione delle entità in `<listObject>` (51 entità), `<listPlace>` (44 entità), `<listOrg>` (34 entità), `<listPerson>`, `<listEvent>` e una lista dedicata ai concetti (`<list type="concepts">`) suddivisa in `abstract`, `trait` e `state`[cite: 3, 4].

## Documentazione nel repository
* `codifica-ner-tei-guiana-ralegh.xml`: file codificato in XML/TEI.
* `Relazione.pdf`: relazione metodologica e di analisi completa (*Laboratorio di Filologia Digitale*).
