NL 233 CNG / NL 313 CNG - VARIABLES FOR REPAINT .CTI FILES

Use the following command to control variables:
[setvar]
variable_name
value

The following list includes all controllable variables. 
Check the manual for more informations.

**** STCP AND GENERIC MODELS ****

option:	VOITH Gearbox buttons
var:	gear_button_type
values:	0 = "classic", white/red background, black characters
	1 = "modern", fully black buttons, white characters

option:	Internal advertisements/stickers (associated to farbschema_tex3)
var:	visible_pub
values:	0 = not visible
	1 = visible

option:	External advertisement boards (associated to farbschema_tex6)
var:	visible_pub_ext
values:	0 = not visible
	1 = visible

option:	Periodical inspection and insurance stamps, Front and Back sticker.
	Optimal for Portuguese buses, for international buses check manual for more information.
var:	visible_stamps
values:	0 = not visible
	1 = visible

**** ONLY FOR GENERIC MODELS ****

option:	Language of the Tecmic (IBIS) device. 
	Please change the farbschema_tex5 texture coherently (check manual).
var:	Tecmic_language
values:	0 = Português
	1 = Deutsch
	2 = English

option:	Color of the external fleet numbers. 
	Positioned in:
	- top right of the front bumper
	- directly below the bottom-right corner of the back window
	- both sides, over the back-most openable windows.
var:	fleet_number_color
values:	0 = all White
	1 = all black
	2 = front and back white, top side black
	3 = front and back black, top side white
	4 = front white, back and top side black
	5 = front black, back and top side white
	6 = front and top side white, back black
	7 = front and top side black, back white
	8 or more = NO FLEET NUMBERS

	value |	FRONT | BACK  | SIDE 
	-----------------------------
	  1   | white | white | white 
	  2   | black | black | black

	  3   | white | white | black
	  4   | black | black | white

	  5   | white | black | black
	  6   | black | white | white

	  7   | white | black | white
	  8   | black | white | black

	  0   NO FLEET NUMBERS
	-----------------------------