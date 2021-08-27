# Frictionless
This is an overview of the frictionless code in this repository.
Section 1:
The first section is the setup. The modules for frictionless, pyjstat, and openpyxl are installed using pip. The necessary libraries are imported, including pandas and pprint.
The dataset is retrieved using a JSON API. The dataset used in this code is from cso.ie, table TFA22
Section 2:
The second section is the application of the frictionless framework. This is divided into four steps; describe, extract, validate and transform. A brief description of each is included in the code as a text box.
Step 1 Describe: the metadata describing the dataset is created and displayed.
Step 2 Extract: The data is read and extracted from the dataset and displayed.
Step 3 Validate: The dataset is checked for errors. A report of the errors contained within the set is created and printed.
Step 4 Transform: A series of transformation is applied which can modify both the data and the metadata. This is the section which produces the most errors. The most common errors seen are to do with the field names contained within the file.
Section 3:
This final section involves dumping the transformed dataset into an excel file for future use. A couple of different methods are explored, including openpyxl, os.path, df.to_excel and frictionless parser.

Results and Conclusion:
The frictionless framework is rather slow and takes a long time to run. It is not suitable for very large datasets such as table THA18, which was previously examined. 
There is a lot that can be done with this code. There are a lot of extra transformation steps that could be included, as well as fixing the errors currently affecting some of the transformation steps. It may also be useful to export the excel file to a specific location for ease of access later.
