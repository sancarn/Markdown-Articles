Hi All,

So we, my friend and I, are working in a markup language we have created (Documentation Markup Language).
You can find the C9 Syntax highlighter [here](https://hastebin.com/jatuhiheqa.js).

I noticed recently that you can add plugins to C9.io and a few days ago I found the [documentation](https://cloud9-sdk.readme.io/docs/modes). 

This leads me to believe that we can use C9 plugins to implement custom syntax highlighters into C9. However there are no examples that I have found of template plugins which implement syntax highlighters

Over the past few days I have been struggling to get this working... If I go to:

my/c9/workspace?debug=2

I have a plugin named "abap2" (i figured to start off with that I'd just use a syntax highlighter already present in ace, as this should be easy to implement (or so I thought...))

![tmp1](https://i.imgur.com/RcOCed6.png)

At the top of abap2.js I have the following:

![tmp2](https://i.imgur.com/FWIpqmA.png)

So as far as I can tell this makes sense. We have abap2.js which has the correct first line, apab2.js requires abap_highlight_rules and everything should follow from there.

When running the plugin in the IDE, if I swap to a file "myFile.abap2", the syntax highlighter is selected from the syntaxes list, however no highlighting is present:

![tmp3](https://i.imgur.com/isz3km8.png)

So here I am a bit clueless as to why this isn't working... Has anyone managed to get custom modes to work in C9? Or are there any existing templates?

Thanks,
~Sancarn
