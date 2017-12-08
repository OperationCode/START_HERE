This is adapted from the [Chef Software](https://github.com/chef/chef-rfc/blob/master/rfc030-maintenance-policy.md#how-the-project-is-maintained) Open Source Maintenance Policy.

# Maintenance Policy

The Maintenance Policy defines how we make decisions about what happens with Operation Code, and associated software projects. It provides the process by which:

* Roadmaps are decided
* Patches are merged
* Disputes are resolved

It is intended to be short, flexible, and clear.

This file is related to the MAINTAINERS and ROADMAP files in Operation Code projects.

# How the project is maintained

This file is the canonical source for how the Operation Code projects are maintained.

# Roles

## Project Lead

* Resolves disputes
* Provides vision and roadmap
* Has universal veto power
* There can be only one

## Lieutenant

* Each component in the project may have at most one Lieutenant
* Provides guidance on future direction for their component
* Resolves disputes within their component
* Has localized veto power
* Plus all the responsibilities of a Maintainer

## Maintainer

* Each component may have multiple Maintainers
* Handles contributions on GitHub - first response to a PR within 48 hours
* Is available in Slack
* Committed to 100% tests passing for your component
* Has full commit/merge access to the relevant repositories

# Roadmap

All project roles should work together to determine the best opportunities for the improvement of the project. This should produce direction for the project, which should be highlighted in the ROADMAP.

As a project role does not necessarily control resources other than their own labor, they should encourage contributors to participate in furthering development of the project toward the goals of the ROADMAP.

Releases should not block on features on the roadmap, rather they should happen as features are completed. The ROADMAP should be organized by general time periods, not by versions
## Example Roadmap entries

```
# 2015 Q2
* Component - Roadmap Item
  Description

# 2015 Q4
* Core - Support for Drone Automation
  Significant time could be saved in enterprise datacenters by using drones to stack and rack servers

# 2016 Q1
* Core - Support Internet of Things
  As a Chef user, I look forward to the singularity
```

# Contributing Patches

## How a patch gets merged

* Open Pull Request (anyone)
* Code reviewed by a Maintainer, Lieutenant, or Project Lead - who will then approve or request changes to the pull request using Github's reviewing tool.
* Merged after approvals by at least two Maintainers for the component(s) affected by your patch.

## Patch Appeals Process

There may be cases where someone wishes to appeal a Maintainer decision. In this event, the "chain of command" for the appeals process is as follows.

* In the event that the actions of a Maintainer are to be appealed, the appeal should be directed to the Lieutenant for that component. As stated above, a Lt retains veto power for the component(s) for which they are responsible.

* In the event that the actions of a Lieutenant are to be appealed, the appeal should be directed to the Project Lead. As stated above, the Project Lead retains universal veto power over all components.

Although Lieutenants and the Project Lead retain veto powers over certain components, use of this veto power is not guaranteed by the submission of an appeal to that person. It is expected that the majority decisions of component Maintainers and Lieutenants will be respected in all but the most exceptional circumstances.

# How to become a...

## Maintainer

* Have patches merged into the relevant component
* Be willing to perform the duties of a Maintainer
* Issue a pull request adding yourself to the MAINTAINERS file for your component
* Receive an absolute majority of existing Maintainers and Lieutenants for your component :+1:
* No veto from the component Lieutenant
* No veto from the current Project Lead

## Lieutenant

* Issue a pull request to the MAINTAINERS file making yourself the Lieutenant
* Be willing to perform the duties of a Lieutenant
* Receive an absolute majority of existing Lieutenants :+1:
* No veto from the current Project Lead

## Project Lead

* Issue a pull request to the MAINTAINERS file making yourself the Project Lead
* Be willing to perform the duties of the Project Lead
* Receive an absolute majority of existing Lieutenants :+1:
* No veto from Operation Code leadership 

# Removing a Maintainer, Lieutenant or Project Lead

If a Maintainer, Lieutenant or Project Lead consistently fails to maintain their responsibilities or becomes disruptive, they can be removed by:

* Issue a pull request removing them from the MAINTAINERS file
* Receive an absolute majority of existing Lieutenants :+1:
* No veto from the current Project Lead

OR

* Issue a pull request removing them from the MAINTAINERS file
* The current Project Lead unilaterally decides to merge pull request

# How to add a component

* Issue a pull request to the MAINTAINERS file describing the component, and making yourself Lieutenant
* Be willing to perform the duties of a Lieutenant
* Receive an absolute majority of existing Lieutenants :+1:
* No veto from the current Project Lead

# How to change the rules by which the project is maintained

* Issue a pull request to this file.
* Receive an absolute majority of existing Lieutenants from the repository MAINTAINERS file :+1:
* No veto from the current Project Lead

# Where can I find the community?

The best place to find contributors is on the Operation Code Slack team. To join the team, join [Operation Code](https://operationcode.org/) and you will receive an email invite to the Slack team.
