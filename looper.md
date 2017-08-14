ci/cd
martin fowloer
typical with agile methodologies.

ci
every change/commit automatically triggers a build.
changes from multiple developers
confidence that build works.

c delivery
every change/commit automatically triggers verification
build on top of ci
unit tests
regression tests
confidence that build output works and could be delivered

c deploymnet
every change/commit automatically triggers deployment
build on top of cd
confidence that customer gets benifits

ci/cd server
------------
montior vcs
detect changes nad trigger job executions
user interface for job access
integration with other tools

looper
------
by walmartlabs
jenkins as foundation
standard ci/cd server at wmt
replace pebl, jenkins, and others
developed and supported by sde team
soon to be open source
sde.walmart.com

features
-------
tight int w github
declarative build definition
  inside source code
  version controlled
automatic tool provisiioning on nodes
complex workflows

not for
batch jobs
report generation jobs
mission critical production
not production ready
not monitored for uptime
status checks
look at BaaS

.looper.yml
main configuration file
defines build executions
located with source code
uses yaml syntax

jenkins with more features
job definition lies with source code

ci.walmart.com
ad user
new item 
github repo url https
default centos slave

build history
console output

warm 
enhanced version of nexus
gec-maven-nexus.walmart.com

oneops integration
add jenkinspan user to organization

slack:
#sde-support
#sde-looper

github:
/devtools/looper
