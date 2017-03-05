Dashboard Me
============

Mostlikely, there is nothing to see here for you.

I got some spare time again and now I want to toy around with a new pet project. fixel.express AI doesnt hook me at the moment.


#### API design:

JWT for auth.

#### Account

**User** -- *POST*:

	- /register
	- /login
	- /unregister

#### Component Lifecycle:

**Create** -- *POST*:

	- /dashboard/<name>
	- /<widget>/<name>

**Show** -- *GET*:
	
	- /dashboard/<name>
	- /<widget>/<name>

**Delete** -- *DELETE*:

	- /dashboard/<name>
	- /<widget>/<name>


#### Component Interaction:

**Modify widget content** -- *PUT* / POST:

	- /<widget>/<identifier>

**Connect UI components** -- *POST*:

	- /link/<dashboard-identifier>/<widget-identifier>

**Disconnect UI components** -- *DELETE*:

	- /link/<dashboard-identifier>/<widget-identifier>


##### Component Introspection:

**List / Brose components** -- *GET*:

	- /widgets
	- /dashboards