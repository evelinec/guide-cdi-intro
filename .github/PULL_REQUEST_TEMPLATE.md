#### What was fixed?  (Issue # or description of fix)

#### Peer Review for `<branch/fork>` to `qa/dev` branch: 
- [ ] Check all the changes
- [ ] Review the changes in http://lgdev1.fyre.ibm.com:4020/guides
- [ ] When PR is good, approve it and tag `Static Guide Admin`

#### Admin to merge into `qa/dev` branch: 
- [ ] Review the changes 
- [ ] Review the changes in http://lgdev1.fyre.ibm.com:4020/guides
- [ ] When PR is good, merge it to the `qa/dev` brach
- [ ] Trigger the `qa` site refresh (~20 minutes)
- [ ] Tag the peer reviewer to review the changes on the `qa` site

#### Peer Review on `qa` or `draft` site: 
- [ ] Verify the readme content on the `qa` site: https://qa-guides.mybluemix.net/guides
  - If guide is a draft, verify the readme content on the `draft` site: https://draft-guides.mybluemix.net/guides
- [ ] Run end-to-end test if necessay, if not, state reason as a comment
- [ ] If everything is good, create a PR from `qa` to `master` with heading `QA to Master: <description>`
- [ ] Assign the PR to the original PR contributor to review
