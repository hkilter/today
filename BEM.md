## BEM Naming Convention

There are some naming conventions to write your code for easy-to-use format such as [BEM][BEM]. Nicolas Gallagher proposed a naming scheme based on BEM in [his article][his_article]. 

The naming convention follows this pattern:

	.block {}             /* Block */  
    .block__element {}    /* Element */ 
    .block--modifier {}   /* Modifier */

**.block** represents the higher level of an abstraction or component.  
**.block__element** represents a descendent of **.block** that helps form **.block** as a whole.  
**.block--modifier** represents a different state or version of **.block**.  

By reading some HTML with some classes in, you can see how – if at all – the chunks are related; something might just be a component, something might be a child, or element, of that component, and something might be a variation or modifier of that component. To use an analogy/model, think how the following things and elements are related:

    .person {}
    .person__hand {}
    .person--female {}
    .person--female__hand {}
    .person__hand--left {}


[BEM]: https://en.bem.info/
[his_article]: http://nicolasgallagher.com/about-html-semantics-front-end-architecture/