#Sample Boundary-Equivalence tables 

## Phone number variable

Variable 		 | Valid case EC 	 | Invalid case EC 	| Boundary and special cases 	| Notes
------------ | --------------  | ---------------- | --------------------------- | -------
Phone number |(\\([+]?[0-9\s]{2,3}\\)\|[+]?[0-9\s]{2,3})?[0-9\s]{7,12} |  		| 1111111 				 | 
             |                 |  					      | 111111111111 								| 
             |                 |  					      | (+09)111111111111  					| 
             |                 |  					      | + 48111111111111  					  |
             |                 |                  | +48 334 226 943             |
             |                 | #digits < 7			| 1111111  								    | 
             |                 | #digits > 15			| 12345234234234234123456 					  |
             |                 | One parenthesis	| (+0999999999999 	   				|
             |                 | empty      			|  								            | 
             |                 | ^[0-9]      			| :/abcdef			              | 

## Email variable

Variable 		| Valid case EC 	| Invalid case EC 	| Boundary and special cases 	| Notes
----------- | --------------- | ----------------- | --------------------------- | -------
Email 			|	[A-Za-z0-9._%+-]{1,20}@[A-Za-z0-9.-]{1,20}.[A-Za-z]{2,6} |  | aAzZ09.%+-aaaadsfscvxcvxcvssfjk@aAaaazaaaa09.ay-defaaaaghijkaaaalmno.azzAZZ	| 
            |                 |                   | g@r.dzd |
            |                 | empty             | |
            |                 | Part before "@" empty | @aaaa.addz |
            |                 | Part before "@" characters > 20 | aAzdfasasfZ09.%+-bcasfasfdefghijkl@z.az |
            |                 | Part after "@" empty | b@.bb | 
            |                 | Part after "@" characters > 20 | af@aAwezewfwefweZ09.%+-bcwefwefwefdefghijkl.azeee |
            |                 | TLD < 2 characters | b@b.b |
            |                 | TLD > 6 characters | c@v.eddAZZd |


## Username, Phone and Email variable test cases created using PICT


Used all pair approach.
1a - first boundary/special case in Username, 2b - second boundary/special case in Phone number etc.

Username | Phone number | Email
-------- | ------------ | -----
 1h|2a|3e 
 1i|2a|3h 
 1a|2d|3b 
 1a|2c|3g 
 1a|2e|3e 
 1a|2f|3d 
 1a|2g|3c 
 1b|2h|3h 
 1a|2i|3i 
 1a|2j|3h 
 1c|2g|3i 
 1d|2e|3i 
 1e|2a|3i 
 1c|2d|3f 
 1h|2e|3b 
 1b|2i|3d 
 1f|2e|3a 
 1g|2f|3f 
 1i|2c|3c 
 1g|2b|3h 
 1a|2h|3a 
 1b|2a|3b 
 1c|2c|3e 
 1d|2i|3h 
 1e|2e|3d 
 1f|2f|3f 
 1g|2b|3c 
 1h|2g|3g 
 1i|2j|3i 
 1e|2d|3c 
 1a|2a|3f 
 1b|2b|3i 
 1c|2a|3g 
 1d|2a|3c 
 1f|2a|3d 
 1g|2a|3a 
 1d|2d|3d 
 1e|2j|3g 
 1h|2h|3c 
 1b|2g|3h 
 1f|2i|3b 
 1e|2c|3g 
 1f|2d|3i 
 1g|2h|3i 
 1h|2c|3i 
 1i|2f|3g 
 1b|2j|3a 
 1d|2j|3b 
 1c|2j|3f 
 1a|2b|3e 
 1e|2i|3g 
 1f|2b|3g 
 1g|2e|3g 
 1h|2i|3f 
 1i|2g|3f 
 1e|2g|3a 
 1c|2h|3b 
 1i|2h|3d 
 1f|2c|3h 
 1b|2d|3g 
 1d|2f|3i 
 1e|2h|3e 
 1g|2i|3e 
 1h|2j|3d 
 1i|2e|3a 
 1h|2f|3b 
 1c|2f|3c 
 1d|2b|3f 
 1b|2c|3d 
 1h|2b|3a 
 1c|2b|3d 
 1b|2f|3e 
 1d|2g|3e 
 1c|2e|3f 
 1g|2f|3a 
 1i|2d|3e 
 1f|2g|3b 
 1g|2c|3b 
 1d|2c|3a 
 1i|2i|3c 
 1c|2e|3h 
 1e|2b|3b 
 1h|2d|3h 
 1b|2e|3c 
 1f|2j|3c 
 1g|2j|3e 
 1c|2i|3a 
 1g|2g|3d 
 1e|2h|3f 
 1d|2h|3g 
 1i|2b|3b 
 1g|2d|3a 
 1e|2f|3h 
 1b|2c|3f 
 1f|2h|3e 