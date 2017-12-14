# plugins

I'm still pondering what to do with this folder. I'm not too fond of the plugin architecture we use, as I found it pretty impenetrable coming on to the project, and still feel that it's more complex than it needs to be without being flexible enough. I'm also aware of the potential avalanche of extra work/regression issues that will come with completely rearchitecting this.

Particular things I don't like:

#### The name

For me, being called 'plugins' confuses things for two reasons:

1. The framework uses plugins; some things in here relate to framework plugins, most things don't.
2. It gives the sense that this folder contains add-on/additional content/functionality. Everything in here is in fact core and required.

With the front-end, I went with the name 'modules' -- this may work here.

#### The API endpoints being hidden away deep in the folder

Although I understand the need for this, it makes working with the API very cumbersome and difficult to follow. Considering everything in here is 'core', this seems slightly unnecessary.
