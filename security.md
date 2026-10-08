# Security Statement

## Intended users

This repository holds my coursework for CSE 3000. It is a fork of the Matt's repo that is meant for only me and Matt to see. 

## Risk assessment
There is very low risk if this repo falls into the wrong hands. The data in the csv files are fake generated data that have no actual meaning. This repo also does not contain any kind of credentials, API keys, tokens or secrets that would be bad if they fell into the wrong hands. 
That being said, there could be some adverse effects if this repo was accessed by a "bad actor":
  - Someone can copy my hw answers, which could mean I get framed for facilitating cheating. 
  - Someone can mess up my whole repo and I have to re-clone Matt's main repo and redo the hw assignments. 
  - Someone tampers with the hw notebook/python files to have something malicious run when I run a hw assignment. 
  
## Steps taken to secure the repo
- I have included a `CODEOWNERS` files that includes Matt and myself as owners of the repo
- Only I have write access, as the repo is a personal fork under my account. There are no added collaborators, so no one else should be able to push to it. 
- I have added the .json file Matt provided on HuskyCT. This ruleset makes it so that nobody can delete main, force-pushes and history rewrites to main are blocked, and changes must come through a pull request that someone listed in `CODEOWNERS` must review. 