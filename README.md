# template-writer
create similar txt documents base on the template and other informations provided.

on python 3, need numpy and dataframe

Functions that intended to be added includes:

1. [yes]replcae the key word directly with "content"
2. [in progress]recognize the python scripts in the template and replace that part with the result of python scripts. 
3. [not yet]more complex replcaement concerning the outputs of other files.
4. [not yet]gennerate multiple files

the working scheme will be:

1. read in the template
2. read in a content csv file 
3. read in the settings
4. search for keywords(marked words) in the template
    -check if there are missing keywords
    -start writing the output according to the setting
        -replace the keyword directly
        -replace the keyword according to the python script string
        -replace the keyword from generated files.

about inputs:
    more details will be included after the implimentation. please refer to the example output before that.
    -template：
        the default mark for keyword or keyword expressions will be /*/* infront and after the keyword 
        other rules for expression will be documented after implimented
    -csv 
        will read by dataframe and thus will follow the rules.
        