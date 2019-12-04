
# 100 Days Of Code - Log
<a name="toc"></a>
### Table of Contents 
|Day|Focus|Day|Focus|
|:---:|:-----:|:---:|:-----:|
|[Day 1](#day-1) **05/12/19**|Bubble Sort, Prime Numbers, Dynamic Allocation|[Day 2](#day-2) **06/12/19**|contnue...|


----------
<a name="day-1"></a>
### Day 1: December 5, 2019 

**Today's Focus**: Practice C [UniquePrimeFactor.c](UniquePrimeFactor.c) library.

**Details**:

 - Playing with [Html Type Provider](http://fsharp.github.io/FSharp.Data/library/HtmlProvider.html) to scrape Vikings episode information (seasons 1-3 in initial attempt) from Wikipedia.
 - Html Type Provider allows you to get compile time type safety and Intellisense from a live website (creates types behind the scenes and explores the HTML as you type)!
 - Great way to explore APIs.

**Examples**: Here is an example of the type provider in action, while it scrapes html information from the season 1 Wikipedia page. I'm able to access html, lists and tables on the fly and then access elements within those structures. Pretty neat stuff! [This](https://en.wikipedia.org/wiki/Vikings_(season_1)#Episodes) is the table I'm accessing from Wikipedia. Also, notice how useful the F# Interactive window is to test your code as your write it :open_mouth:

![Day 1 Example](https://raw.githubusercontent.com/jasondown/100-days-of-code/master/images/day1_htmlprovide.gif)

**Link to work**: [Github](https://github.com/jasondown/FunWithFSharpData/)

[Table of Contents](#toc)

----------
 <a name="day-2"></a>
### Day 2: January 3, 2018

**Today's Focus**: Continue learning [FSharp.Data](http://fsharp.github.io/FSharp.Data/) library.

**Details**:

 - Refactored some of the Vikings episode Wikipedia scraper code. I figured out how to pass the [Html Type Provider](http://fsharp.github.io/FSharp.Data/library/HtmlProvider.html) as a parameter in a function so I could make some code reuse. Instead of instantiating one per season directly, I wrapped the type, providing the season 1 table as sample data. Then I used the *Load* function to create each season. Changes can be seen [here](https://github.com/jasondown/FunWithFSharpData/commit/0e79445abaa236e128384db03ff4080d425d7198). *NOTE: There was a bug in the refactored code where all episodes were being reported as season 1. This has been fixed*.
 - Created another example using the [JSON Type Provider](http://fsharp.github.io/FSharp.Data/library/JsonProvider.html) and the free [IEX Trading API](https://iextrading.com/developer/docs/#getting-started) to grab a bunch of *tech giant* stock quote information and display the current trading price. Again, you get Intellisense from the JSON returned from the API.

**Examples**: Here is an animated GIF showing the stock quote code in use with F# Interactive:

![Day 2 Example](https://raw.githubusercontent.com/jasondown/100-days-of-code/master/images/day2_jsonprovider.gif)

**Links to work**:

 - [Main repository](https://github.com/jasondown/FunWithFSharpData)
 - [Vikings episode scraper](https://github.com/jasondown/FunWithFSharpData/blob/master/FunWithFSharpData/HtmlProviderExample.fsx)
 - [Stock quote lookup](https://github.com/jasondown/FunWithFSharpData/blob/master/FunWithFSharpData/JsonProviderExample_StockQuotes.fsx)


[Table of Contents](#toc)

----------
