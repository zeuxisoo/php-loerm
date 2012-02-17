### License

	The BSD 2-Clause License

### API

###### Generate single word

	Lerom::word()

###### Generate 10 words

	Lerom::words(10)

###### Generate one sentence

	Lorem::sentence()

###### Generate 10 sentences

	Lorem::sentence(10)

###### Generate date (Default format: %a %b %d, %Y)

	Lorem::date()

###### Generate date (By format)

	Lorem::date("%a %b %d")

###### Generate name (first_name last_name)

	Lorem::name()

###### Generate first name only

	Lorem::first_name()

###### Generate last name only

	Lorem::last_name()

###### Generate email

	Lorem::email()

###### Generate image

	Lorem::image("200x200" [, array $options])

	<img src="<?php echo Lorem::image("200x200")?>">

**About the options**

`text`: default text  

`color`: text color  

`background_color`: background color  

`random_color`: generate background color and font color randomly (boolean)  

**For example**

	Lorem::image("200x200", array("random_color" => true, "text" => 1234))
	Lorem::image("200x200", array("background_color" => "000", "text" => 1234))
	Lorem::image("200x200", array("color" => "F00", "text" => 1234))
	Lorem::image("200x200", array(
		"background_color" => "000", 
		"color" => "F00", 
		"text" => 1234
	))