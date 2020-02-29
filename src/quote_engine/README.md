# quote_engine module


This module contains QuoteModel, IngestorInterface(abstract class), Ingestor, PDFImporter, CSVImporter, TXTImporter and DOCXImporter classes.
The classes PDFImporter, CSVImporter, TXTImporter and DOCXImporter realize IngestorInterface.


## Roles and Responsibilities


QuoteModel - This is a class for creating quote object. The class takes quote and the author and creates a quote object from it.


IngestorInterface - This acts as base class for PDFImporter, CSVImporter, TXTImporter and DOCXImporter. It defines abstract method parse.


Ingestor - This class encapsulates all 4 file importer classes.


PDFImporter, CSVImporter, TXTImporter and DOCXImporter - These classes realize IngestorInterface and return quotes from pdf, csv, txt and docx file formats respectively.



## Dependencies



Libraries ABC, subprocess, random, python-docx, pandas and os are required for using this module.



## How to use


Ingestor.parse(file_path)


The Ingestor class takes the file path and calls the right class to read contents from the file and returns list of quotes after parsing.


