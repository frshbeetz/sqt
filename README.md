# sqt
sqt - a stock quote grabber in bash

The script sqt crafts a url that is compatible with the yahoo finance csv request and gives you the data in return.  I've made it so that it reminds you of a few basic options that can be included in the url, but you should be able to include any from a site like this: http://www.canbike.org/information-technology/yahoo-finance-url-download-to-a-csv-file.html

Roadmap:

    [ ] I hope to have it display headings based on the l1,g,h etc.. options 
        at the top of the columns in comparative mode.
 
    [ ] I'd like to make the default function spit a quote out simply by 
        not giving an option and providing a ticker as an argument.
 
    [ ] The comparative mode requests a number of stocks to compare up front, 
        mainly because I am a lousy programmer.  I'd like it to ask for tickers until 
        it gets some special input, and then move along to the next task.
  
Notes: 

  requires 

    figlet (easy to fix this with a look at the code, if you hate fun...)
    curl (I'm sure there's other ways to do it, but curl works)
    
  warnings

    this software comes with no warranty or even an advisement to run it. it may: 
    burn down your home, kick your dog, or even sleep with your spouse, 
    and i refuse to take responsibility if you execute it.
    
    there exists specifically one "rm -rf /tmp/output.tbl" statement, 
    this is where comparative mode saves it's data, it removes the existing file as 
    part of the initialization. if this is safe or not, i have no idea.
  
  acknowledgments
  
    i remember seeing the original url with curl method in a thread on commandlinefu, 
    and ultimately just wanted to make it a bit more fun and interactive.
  
    thanks to sintaxerror for explaining how to get the terminal width programmatically, 
    and for showing me how wonderful defining functions can be.
