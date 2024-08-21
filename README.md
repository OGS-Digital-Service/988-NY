# 988-NY
NYS 988 Static Component Generator

Demo site available at https://988-ny.netlify.app

- bootstrap 3 is a dependency, built into the omhweb theme. There's a duplicate reference to the bootstrap js in their footer, which causes some unpredicatable behavior. This was not our task to fix.

- html and css are the only files needed for production.

- Final production ready assets are available in the _DISTRIBUTION folder.

- All relative link urls should be changed to full path .html urls in the production code. omhweb template do not resolve directory indexes.

- pa11y automated reports are available at https://988-ny.netlify.app/pa11y-reports - they contain errors that pertain to the omhweb template and show no errors in axecore or htmlcs for our static component code. 

- components have been manually checked for accessibility conformance using keyboard navigation with screen readers NVDA & VoiceOver as well as numerous automated tests that will be outlined in another repo. 

- New components can be generated by using the provided templates and local builds of 11ty using the render layout.

- image path for distribution: /omhweb/bootstrap/img/*

- Need Help? email us at Digital.Services@ogs.ny.gov