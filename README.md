


**Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.**  

I would put my automated tests within a Github Action that runs whenever code is pushed. This makes for continuous integration, as automated tests catch on any issues before they make more complicated buggy code. Having this system will make the workflow consistent and safe for quality.   
Testing locally is great as well, but the local environment is able to have differnt environments compared to the environment provided by github actions, as there can be many things that can affected locally by your own machine, which may affect your perceived status of your code. There is also some possible human error, as sometimes people may forget to manually test their code locally before pushing their code.   

**Would you use an end to end test to check if a function is returning the correct output? (yes/no)**  

No, I would not use an end to end test to check if a function is returning the correct output. End to End testing is supposed to emulate user actions throughout, not for a simple function test that a unit test can do.   

**What is the difference between navigation and snapshot mode?**   

The difference between navigation and snapshot mode  is that navigation mode analyszzes the page right after it reloads, focusing on the performance metrics right after the initial loading. Snapshot mode analyzes the page in the current state of the page. This is different from navigation mode as snapshot mode can be used on pages that may have some changes after some interactions.   

**Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.**

Some ways to improve thr CSE 110 shop site based on the Lighthouse results:
- Lighthouse results tell us there are missing things such as `<meta name="viewport">`, which tells us that `<meta name="viewport">` not only optimizes your app for mobile screen sizes, but also prevents a 300 millisecond delay to user input.  
Another one is that `<html> element does not have a [lang] attribute.`
Lighthouse tells us if a page doesn't specify a lang attribute, a screen reader assumes that the page is in the default language that the user chose when setting up the screen reader. If the page isn't actually in the default language, then the screen reader might not announce the page's text correctly.  
The website also does not have a meta description.
Lighthouse tells us that meta descriptions may be included in search results to concisely summarize page content.
- Lighthouse results tell us that images were larger than their displayed size. Images that are appropriately-sized to save cellular data and improve load time.
- Lighthouse results show that we can minify the JavaScript used on the website, up to potential savings of 44 KiB. Minifying JavaScript files can reduce payload sizes and script parse time. 