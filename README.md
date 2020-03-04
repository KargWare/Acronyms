# Acronyms by KargWare

[Jekyll](https://jekyllrb.com/) Acronyms for the blog [Notes by KargWare](https://notes.kargware.com). The project is hosted on [GitHub](https://github.com/KargWare/Acronyms).

## Values for a acronym

* date -> When was the acronym added
* key -> The acronym
* value -> The long value of the acronym

## VScode Snippet

All snippet files need to be placed inside the `.vscode` folder.  

jekyll.code-snippets

```json
{
	"Add new acronym":{
		"prefix": "kw-jekyll-acronym",
		"scope": "markdown",
		"body": [
			"---",
			"date: $CURRENT_YEAR-$CURRENT_MONTH-$CURRENT_DATE $CURRENT_HOUR:$CURRENT_MINUTE:$CURRENT_SECOND +0200",
			"key: \"${TM_FILENAME_BASE/(.*) - (.*)/$1/}\"",
			"value: \"${TM_FILENAME_BASE/(.*) - (.*)/$2/}\"",
			"---"
		],
		"description": "Add new acronym on website collection"
	}
}
```
