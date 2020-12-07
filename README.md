# git-flow-sugar

### Installation

#### Using homebrew

1. brew tap bepro-company/brew
2. brew install bepro-company/brew/git-flow-sugar
3. brew upgrade bepro-company/brew/git-flow-sugar

#### Manual install

1. download repository or repository sources.
2. Add or symlink git-* scripts to PATH.

### Usage

#### Create a new feature branch from develop

```bash
# for DATACENTER-715 Jira ticket
git-feature 715 jira_integration  # DATACENTER is a default project
git-feature DATACENTER-715 jira_integration

# for tickets of RESEARCH, EDITOR projects
git-feature RESEARCH-1 camera_sync
git-feature EDITOR-1 3d_player
```

#### Create a new hotfix branch from master
```bash
# for DATACENTER-715 Jira ticket
git-hotfix 715 jira_integration  # DATACENTER is a default project
git-hotfix DATACENTER-715 jira_integration

# for tickets of RESEARCH, EDITOR projects
git-hotfix RESEARCH-1 camera_sync
git-hotfix EDITOR-1 3d_player
```

#### Push commits and make a pull request

```bash
# Jira ticket will be attached in body automatically
# If a base branch is omitted, it aims to develop 
git-pr
git-pr master
```
