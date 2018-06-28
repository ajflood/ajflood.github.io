# BibTeX Templates

|Tag | Use case |
|-----------------|
|[@article](#@article) 				|  An article from a magazine or a journal. 	|
|[@book](#@book) 					| A published book	|
|[@booklet](#@booklet) 				| bound work without a named publisher or sponsor.	|
|[@inbook](#@inbook) 				| section of a book without its own title.	|
|[@incollection](#@incollection) 		| A section of a book having its own title.	|
|[@inproceedings](#@inproceedings) 	| An article in a conference proceedings.	|
|[@manual](#@manual) 				| Technical manual	|
|[@mastersthesis](#@mastersthesis) 	| Master's thesis	|
|[@misc](#@misc) 					| Template useful for other kinds of publication	|
|[@online](#@online) 				| An unpublished article, book, thesis, etc.	|
|[@phdthesis](#@phdthesis) 			| Ph.D. thesis	|
|[@proceedings](#@proceedings) 		| The proceedings of a conference.	|
|[@techreport](#@techreport) 			| Technical report from educational, commercial or standardization institution.	|
|[@unpublished](#@unpublished)		| An unpublished article, book, thesis, etc.	|
|---------------------|


### @article 
An article from a magazine or a journal.
Required fields: author, title, journal, year.
Optional fields: volume, number, pages, month, note.
```
@article{,
	author	= {},
	title	= {},
	journal	= {},
	year		= "XXXX",
	
	volume	= {},
	number	= {},
	pages	= {},
	month	= {},
	note	= {},
}
```

### @book 
A published book
Required fields: author/editor, title, publisher, year.
Optional fields: volume/number, series, address, edition, month, note.
```
@book{,
	author    = {},
	title     = {},
	publisher = {},
	year      = "XXXX",
	
	volume   = {},
	number   = {},
	series   = {},
	address  = {},
	edition  = {},
	month    = {},
	note     = {},
}
```

### @booklet 
A bound work without a named publisher or sponsor.
Required fields: title.
Optional fields: author, howpublished, address, month, year, note.
```
@booklet{,
	title     = {},
	
	author   = {},
	howpublished   = {},
	address  = {},
	year      = "XXXX",
	month    = {},
	note     = {},
}
```

### @inbook 
A section of a book without its own title.
Required fields: author/editor, title, chapter and/or pages, publisher, year.
Optional fields: volume/number, series, type, address, edition, month, note.
```
@inbook{,
	author	= {},
	editor	= {},
	title	= {},
	chapter	= {},
	pages	= {},
	publisher= {},
	year	= {},
	
	volume	= {},
	number	= {},
	series	= {},
	type	= {},
	address= {},
	edition= {},
	month	= {},
	note	= {},
}
```

### @incollection 
A section of a book having its own title.
Required fields: author, title, booktitle, publisher, year.
Optional fields: editor, volume/number, series, type, chapter, pages, address, edition, month, note.
```
@incollection{,
	author	= {},
	title	= {},
	booktitle= {},
	publisher= {},
	year	= {},
	
	editor	= {},
	volume	= {},
	number	= {},
	series	= {},
	type	= {},
	chapter= {},
	pages	= {},
	address= {},
	edition= {},
	month	= {},
	note	= {},
}
```

### @inproceedings 
An article in a conference proceedings.
Required fields: author, title, booktitle, year.
Optional fields: editor, volume/number, series, pages, address, month, organization, publisher, note.
```
@inproceedings{,
	author		= {},
	title		= {},
	booktitle		= {},
	year			= {},
	
	editor		= {},
	volume		= {},
	number		= {},
	series		= {},
	pages		= {},
	address		= {},
	organization	= {},
	publisher	= {},
	month		= {},
	note		= {},
}
```

### @manual 
Technical manual
Required fields: title.
Optional fields: author, organization, address, edition, month, year, note.
```
@manual{,
	title		= {},
	
	author		= {},
	organization	= {},
	address		= {},
	edition		= {},
	year		= {},
	month		= {},
	note		= {},
}
```

### @mastersthesis 
Master's thesis
Required fields: author, title, school, year.
Optional fields: type (eg. "diploma thesis"), address, month, note.
```
@mastersthesis{,
	author    = {},
	title     = {},
	school    = {},
	year      = "XXXX",
	
	type     = "diploma thesis",
	address  = {},
	month    = {},
	note     = {},
}
```

### @misc 
Template useful for other kinds of publication
Required fields: none
Optional fields: author, title, howpublished, month, year, note.
```
@misc{,
	author    = {},
	title     = {},
	howpublished = {},
	year     = "XXXX",
	month    = {},
	note     = {},
}
```

### @online
An unpublished article, book, thesis, etc.
Required fields: author/editor, title, year/date, url.
Optional fields: subtitle, titleaddon, language, version,  note, organization, date, month, year, addendum.
```
@online{,
	author		= {},
	title	= {},
	year		= {},
	url		= {},
	
	subtitle	= {},
	titleaddon = {},
	language	= {},
	version	= {},
	note		= {},
	organization = {},
	date		= {},
	month	= {},
	addendum	= {},
}
```

### @phdthesis 
Ph.D. thesis
Required fields: author, title, year, school.
Optional fields: address, month, keywords, note.
```
@phdthesis{,
	author		= {},
	title		= {},
	school		= {},
	year			= {},
	
	address		= {},
	month		= {},
	keywords		= {},
	note		= {},
}
```

### @proceedings 
The proceedings of a conference.
Required fields: title, year.
Optional fields: editor, volume/number, series, address, month, organization, publisher, note.
```
@proceedings{,
	title		= {},
	year			= {},
	
	editor		= {},
	volume		= {},
	number		= {},
	series		= {},
	address		= {},
	organization	= {},
	publisher		= {},
	month		= {},
	note			= {},
}
```

### @techreport 
Technical report from educational, commercial or standardization institution.
Required fields: author, title, institution, year.
Optional fields: type, number, address, month, note.
```
@techreport{,
	author    = {},
	title     = {},
	institution = {},
	year      = "XXXX",
	
	type     = {}, 
	number   = {},
	address  = {},
	month    = {},
	note     = {},
}
```

### @unpublished 
An unpublished article, book, thesis, etc.
Required fields: author, title, note.
Optional fields: month, year.
```
@unpublished{,
	author	= {},
	title	= {},
	note	= {},
	year	= {},
	month	= {},
}
```

