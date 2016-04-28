## BEM Naming Convention

There are some naming conventions to write your code for easy-to-use format such as [BEM][BEM]. Nicolas Gallagher proposed a naming scheme based on BEM in [his article][his_article]. 

The naming convention follows this pattern:

	.block {}    
    .block__element {}    
    .block--modifier {}


.block represents the higher level of an abstraction or component.  
.block__element represents a descendent of .block that helps form .block as a whole.  
.block--modifier represents a different state or version of .block.  

The reason for double rather than single hyphens and underscores is so that your block itself can be hyphen delimited, for example:

.site-search {} /* Block */
.site-search__field {} /* Element */
.site-search--full {} /* Modifier */
The point of BEM is to tell other developers more about what a piece of markup is doing from its name alone. By reading some HTML with some classes in, you can see how – if at all – the chunks are related; something might just be a component, something might be a child, or element, of that component, and something might be a variation or modifier of that component. To use an analogy/model, think how the following things and elements are related:

.person {}
.person__hand {}
.person--female {}
.person--female__hand {}
.person__hand--left {}
The top-level block is a ‘person’ which has elements, for example, ‘hand’. A person also has variations, such as female, and that variation in turn has elements. This again, but written in ‘normal’ CSS:

.person {}
.hand {}
.female {}
.female-hand {}
.left-hand {}
These all make sense, but are somewhat disconnected. Take .female for example; female what? What about .hand; a hand of a clock? A hand in a game of cards? By using BEM we can be more descriptive but also a lot more explicit; we tie concrete links to other elements of our code through naming alone.


Enter text in [Markdown](http://daringfireball.net/projects/markdown/). Use the toolbar above, or click the **?** button for formatting help.

[BEM]: https://en.bem.info/
[his_article]: http://nicolasgallagher.com/about-html-semantics-front-end-architecture/