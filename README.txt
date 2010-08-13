ABOUT 960 LESS (V 0.2)

960 LESS is an adaption of the 960 Grid System available at http://960.gs. This adaption is done to make use of LESS Mixins to, in theory, allow for less code to be used in the creation of a site. The flexibility of the mixins allows for pretty much any grid system to be usable, with margins of 10px per column. This allow, in theory, 2, 3, 4, 5, 6, 8, 10, 12, 15, 16, 20, 24 or more columns to be used without having to create excessive amounts of code.

EXAMPLE OF USE

The default number of columns is set to 24. This is the first proper line of the .less file, and can be changed to whatever your personal preference is. The first thing you need to do is define a wrapping element that has a width. This is done by adding the .container() mixin to an element:

#container{
  .container();/* This sets up the basic 960 Container for columns to use. */
}

To create columns you call the mixin .grid(). There are 2 values required for this mixin. The first is the total number of columns you want in your grid, the second is the number of columns you want this element to have. To take an example from how the 960 Grid typically works, here are some examples of how 960 LESS can be used to replicate some of the basic 960 Grid.

.grid_1{    
	.grid(24,1); 
} 

.grid_2{    
  .grid(24,2); 
}

.grid_3{    
	.grid(24,3); 
}
    
Additional options, such as prefix, suffix, alpha and omega (common elements within the 960 Grid System) are also available for use, as can be seen in the following example:

.grid_1{    
	.grid(24,1);  
	.suffix(24,2);  
	.alpha;
}             

VERSION HISTORY

0.1 - Basic 960 Functionality
0.2 - Added options for prefix and suffix elements to allow better alignment of elements [First Version on GitHub]