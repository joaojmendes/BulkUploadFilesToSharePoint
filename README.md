I need upload to SharePoint Online Site about 7000 files to a document library as setup of ECM Project, and I develop a tool that permit upload files automatically based on information defined in CSV file.

The power user classify the file, defining Content Type and content type metadata, file path, destination document library, in my case we use the content organizer,  and content organizer rules to route files for their destination. The document library is a DropOff library, but we can specify any library as destination.

the csv file has fill rules that have to be met, particularly with regard to specifying the metadata associated with the file.

The rules are:

The first 3 columns are fixed , the first column define the local (pc) file Path to upload,  second, the content type name and the third is SharePoint Document Library (Destination).

the fourth and next columns are variable and define the metadata associated to content type. The columns must have the internal names of columns in SharePoint Document Library and their values must be compatible with columns.

For Metadata Columns the values must be in format "termgroup|termset|term",

For lookup Columns the values must be the value of reference column defined on Lookup Column. 

For Date Columns the values must be in format "pt-PT"  I will check if the current (PC or Server ) culture is equal.

We must have one file for each content type that we want upload.

You must change the script for your needs, use as a reference .

 




