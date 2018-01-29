This past week, I learned a lot about CSS that I hadn't previously understood.  Brian's workshop in CSS helped reinforce three concepts:   

##Nesting
	SASS can mirror the mapping of HTML markup
	To avoid creating an unmanageable indented tree effect, partials are used to represent more nuanced pieces of the larger picture.

##Parials
	These are really where my mind is going with CSS.  Once the base formatting is laid out, these allow the modularity to come to life.
	40-50 lines is the limit for a partial, so keep breaking these down into smaller pieces

##Mixins
	With legacy browsers, it is important to build backwards compatibility into your CSS.
	It is worthwhile to create a sticky mixin file that you copy from project to project as you develop a list of components that should be commonly addressed 

It was useful to reinforce the idea that you should lean on modularity in your .scss files so that you can keep unique details clearly connected to the components they are affecting.  