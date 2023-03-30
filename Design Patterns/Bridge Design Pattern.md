> **Bridge** is a structural design pattern that lets you split a large class or a set of closely related classes into two separate hierarchies—abstraction and implementation—which can be developed independently of each other.

![[Bridge Pattern Diagram]]

So instead of creating all possible classes combination of 2 sets of classes like 
**LongFormBookView**, **LongFormAlbumView**, **ShortFormBookView**, **ShortFormAlbumView** etc. we have created 
two abstracts that have composition in between.
Now we can create an object of LongFormView that has a Book Object.

The Interface will have some methods that will be used by Abstraction Class