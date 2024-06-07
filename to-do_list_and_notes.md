# to-do list  and notes
>[!comment] (which shows that almost [every project needs a plan](https://wiki.openglobalmind.com/ogm_stewardship/project_plans/template_for_project_(how_to_use)))

- this may turn out to be an ad-hoc list of imagined plans  

1. primary current experiment is to use this vault to debug using MassiveWikiBuilder to construct and deploy the website to Github Pages.
		- several attempts to construct a working and understandable `github-pages.yml` file have failed; so that's discouraging ....  
		- 

2024-06-03:
 - finally have some success with build-and-deploy using a github-action
 - major drawbacks are:
	 - 1. CSS is not applied to the webpages even though it appears to be sitting right there
	 - 2. the repo name needs to be at the front of all the hrefs, and that needs to be tracked down inside `mwb.py`  

2024-06-07:  
 - with PK's help we have some notions of clarifying the properties our model of a MassiveWiki and associated static website  
	 - specifically, the website root directory and it's place in links and wikilinks -- it takes some thinking ....
