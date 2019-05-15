#### What was fixed?  (Issue # or description of fix)

_____
#### PR from `<branch/fork>` to `qa/dev` branch 

#### Peer review for `<branch/fork>` to `qa/dev` branch: 
- [ ] Check all the changes
- [ ] Review the changes in http://lgdev1.fyre.ibm.com:4020/guides
- [ ] When PR is good, approve it and tag `OpenLiberty/static-guide-admin`

#### Admin to merge into `qa/dev` branch: 
- [ ] Review the changes 
- [ ] Review the changes in http://lgdev1.fyre.ibm.com:4020/guides
- [ ] When PR is good, merge it to the `qa/dev` brach
- [ ] Trigger the `qa` site refresh (~20 minutes)
- [ ] Tag the peer reviewer to review the changes on the `qa` site

#### Peer review on `qa` or `draft` site: 
- [ ] Verify the readme content on the `qa` site: https://qa-guides.mybluemix.net/guides
  - If guide is a draft, verify the readme content on the `draft` site: https://draft-guides.mybluemix.net/guides
- [ ] Run end-to-end test if necessay, if not, state reason as a comment
- [ ] If everything is good, create a PR from `qa` to `master` with heading `QA to Master: <description>`
- [ ] Assign the PR to the original PR contributor to review

_____
#### PR from `qa` to `master` branch ####

- [ ] PR contributor to verify the `QA to Master` PR is good 
- [ ] Tag `OpenLiberty/static-guide-admin` after approving the `QA to Master` PR

#### Admin to merge `QA to Master` PR: 
- [ ] Verified changes are good and approved
- [ ] Label `Green to master` or `Yellow to wait` for depending PRs

At 4PM daily, check [query] with `Green to master` PRs, merge all, then request ol.io site refresh. 
- [ ] Tag peer reviewer to verify changes on `openliberty.io` site

#### Peer Review on `openliberty.io` site: 
- [ ] Review changes on `openliberty.io` site
- [ ] Run `mvn install` under the `finis`h directory for most guides, or run `mvn package` for the kube guides
- [ ] Verify that daily build test is run accurately and successfully 
