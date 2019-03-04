# php_random_names
Here is A PHP 7 class to provide random names in several formats. Another PHP7 random name generator! Currently only does first names. I found myself needing to generate random names and could not quickly find a simple PHP class to do so, so here we are.

Can return a single name in string, CSV as string, list as string, or array. Included is a default list of 4950 names.

It can even generate a random sized list, CSV, or array of names if you want that, which is default when calling functions. It will create a specific sized list, CSV or array of names if you tell it to.

## Getting Started
Be running PHP 7 on your web server.

Download names.php to the appropriate directory.

Create a $names object.

Call functions as needed.


## Available Functions
$names->return_random_name() - Returns a single name as a string.

$names->return_list_random_names($num = 0) - Returns a newline delimited list of names as string. If no number is specified, list size is random. If a number is specified, it generates that exact number of names in the list.

$names->return_csv_random_names($num = 0) - Returns Comma Seperated Value, or CSV, list of names as string. If no number is specified, list size is random. If a number is specified, it generates that exact number of names in the list.

$names->return_array_random_names($num = 0) - Returns an indexed array of names. If no number is specified, list size is random. If a number is specified, it generates that exact number of names in the array.



## Examples

```
<?
//add names file

require_once("names.php");

//create $names object

$names = new names();



//return a single random name as a string

$names->return_random_name();

Reults:




//return a random sized list of names as a string

$names->return_list_random_names();

Reults:


//return a CSV of 8 names as string

$names->return_csv_random_names(8);
Results:



//return an array with 9 names

$names->return_array_random_names(9);


?>
```

The above would result in:

Single name:
```
Penelope
```

List:
```
Rea
Merissa
Charleen
Kanya
Lucilia
Mariejeanne
Misti
Danette
Druci
```

CSV result:
```
Eada,Linn,Vicki,Aili,Timothea,Danell,Wendeline,Janine
```

Array result:
```
Array
(
    [0] => Augusta
    [1] => Collie
    [2] => Bel
    [3] => Jackquelin
    [4] => Reggi
    [5] => Marylin
    [6] => Miran
    [7] => Merrie
    [8] => Harrie
)
```


## Acknowledgments
The original list of names is from Moby Word Lists by Grady Ward, website: https://www.gutenberg.org/ebooks/3201

## Misc
I did not do spell check.

## License
```
##############################LICENSE################################
#Copyright (c) 2019 Eric Wamsley.                                   #
#All rights reserved.                                               #
#                                                                   #
#Redistribution and use in source and binary forms are permitted    #
#provided that the above copyright notice and this paragraph are    #
#duplicated and viewable in all forms and that any documentation,   #
#advertising materials, and other materials related to such         #
#distribution and use acknowledge that the software was developed   #
#by ERIC WAMSLEY. THIS SOFTWARE IS PROVIDED "AS IS" AND WITHOUT     #
#ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, WITHOUT LIMITATION,  #
#THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A        #
#PARTICULAR PURPOSE.                                                #
##############################LICENSE################################
```
