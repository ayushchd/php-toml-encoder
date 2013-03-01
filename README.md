PHP TOML Encoder
===============

PHP encoder for Tom's Obvious, Minimal Language (TOML) ( https://github.com/mojombo/toml )


Usage
-----

```
require("../src/toml.php");

$arr = array (
	'a' => 1,
	'b' => array (1, 2, 3),
	'c' => array ('x' => 'apple', 'y' => array(4, 5, 6)),
	'd' => true
	);

$encoder = new Toml_Encoder();
echo $encoder->encode($arr);
```


Contribute
----------

TOML specs are still changing so if there is something that has been added and/or I have missed, feel free to send me a pull request


TODO
----

- Throw exceptions when invalid arrays are passed (e.g. arrays with mixed data types)
- Test


License
-------

MIT