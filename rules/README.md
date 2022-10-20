# Word Processing Rules
   
Useful rules for [Hashcat](http://hashcat.net), [HCRE](https://github.com/llamasoft/HashcatRulesEngine) and [JTR](https://openwall.com/john) 

They fall into three categories:

	- Appension/prepension
	- Word transformation
	- Wordlist trim

## Appension/prepension of a sequence
Rules from this category add a prefix or suffix to the input word.

`NAME` |`DESCRIPTION`
--- | ---
&nbsp;[append/prepend]_season.rule| &nbsp;Prepend or append names of the seasons
&nbsp;[append/prepend]_year.rule| &nbsp;Prepend or append years from 2010 to 2020

## Word transformation
Those rules perform common transformations of input words, such as letter case swap, special characters replacement etc.

`NAME` | `DESCRIPTION`
--- | ---
&nbsp;revert.rule| &nbsp;Revert every character 
&nbsp;leet.rule | &nbsp;Convert "leet" to "l337"
&nbsp;cap_all.rule | &nbsp;Convert every character to uppercase
&nbsp;cap_first.rule | &nbsp;Capitalize first character
&nbsp;cap_invert.rule | &nbsp;Lowercase first character and uppercase the rest
&nbsp;duplicate.rule | &nbsp;Duplicate a word
&nbsp;ru_convert.rule | &nbsp;Replace ASCII characters with corresponding Cyrylic alphabet
&nbsp;first\_last\_char_remove.rule | &nbsp;Remove first and last character
&nbsp;swap\_last\_two_chars.rule | &nbsp;Swap two last characters 
&nbsp;swap\_first\_two_chars.rule | &nbsp;Swap two first characters
&nbsp;num\_special\_convert.rule | &nbsp;Replace numbers with special characters 

## Wordlist trim
Use those rules to remove all words from dictionary that do not satisfy prerequisities of a rule.

`NAME` | `DESCRIPTION`
--- | ---
&nbsp;reject_8.rule| &nbsp;Remove words of length smaller than 8 
&nbsp;reject\_8_16.rule | &nbsp;Remove words of length smaller than 8 and greater than 16










