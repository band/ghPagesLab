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

2024-06-09:
 - figured out my own Python coding error and with some hard-coding on
   the not-wikilinks local pages links in the Sidebar.md file gh-pages
   works. The local page links issue needs a solution.  
 - i made one pass at updating all-pages.html to fit with the dolce
   theme, but the sidebar is not displaying.  
   
 - next step is to sort the local webpage link problem.
 - also, update all the links that require `websiteroot`  

2024-06-10:  
 - `websiteroot` parameterized in most of the code  
 TODO: update all the `hrefs` generated in MassiveWikiRenderer  
 
 - decided on adding `websiteroot` to the command-line arguments  
   rationale: only need to change `gh-pages.yml` file; `netlify.toml`
   can stay the same.  
   
 - TODO: the current test wiki and Obsidian vault only has a few files in
   it; further testing required.  

 - some other thoughts:  
	 - another rationale for command-line `websiteroot` specification is that `mwb.yaml` can be used for multiple web publication sites without change  
	 - Note: this does mean that PyPI module initialization might need to query for expected deployment method (and where would that info go if not into `mwb.yaml`?)  
	 - there are questions to be resolved about how to help the user of the system set up, or modify already set up, configurations.  
   

 
