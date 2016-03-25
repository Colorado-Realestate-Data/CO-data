The 2013 data is from oct 22 2013
2009 is from Nov 10 2009

The data seems to be endoced in windows-1252


There are some non utf-8 compatible (or they seem to cause problems) characters for exmaple "¬" and "¢".


These can be removed using code such as


line.decode('utf-8', 'ignore').split(',')
