# php_random_names
I found myself needing to generate random names and could not quickly find a simple PHP class to do so.

Here is A PHP 7 class to provide random names in several formats. 
Can be a single name in string, CSV as string, list as string, or array. Included is a default list of 4950 names.


To create a names class object: $names = new names();
To return a single random name from the $names object: $names->return_random_name();
To return a random sized string list of random names: $names->return_list_random_names();
To return a list of 50 names: $names->return_list_random_names(50);
To return a random sized CSV string of random names: $names->return_csv_random_names();
To return a CSV of 85 random names: $names->return_csv_random_names(85);
To return a random sized array of random names: $names->return_array_random_names();
To return an array of 5000 random names: $names->return_array_random_names(5000);


Example:

//add names file
require_once("names.php");
//create $names object
$names = new names();

//return a single random name as a string
$names->return_random_name();