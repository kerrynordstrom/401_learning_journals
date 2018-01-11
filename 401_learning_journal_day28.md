It's been awhile since we've written a learning journal, but I'll try to summerize some things I've learned recently.

I learned today that when we are passing state from one component to another as props that we can basically name the state to be passed anything and then call this within the component it's being passed to.  For example, 
```		  
<NoteList 
allNotes={this.state.notes} 
handleNoteRemoval={this.handleRemoveNote}/>
```

passes the notes array from this.state as `allNote` and the method handleRemoveNote attached to `this` constructor as `handleNoteRemoval`.

Previously, I had assumed that the prop reassignment was also a method or property that would be called somewhere else so I was all kinds of confused until this afternoon.

Another thing I learned recently is that if you are unable to get a promise to return from some method or library, you can easily force it to return a promise with `return new Promise(resolve, reject)`.  Then within that constructor, `return resolve()` Simple....

Lastly...I'm super happy that we're on React and that I can practice a modern, super applicaable technology.  The browser dev tools are awesome and I'm having a great time exploring the results as things get posted to the DOM and are held in state/props.