  This is a simple role which pulls down code from a git repo, this may be useful when you are deploying code and need to ensure that your codebase is up to date on your servers :) Below is a sample playbook that shows the usage. Feel free to PR and fork :D
  
    ---
    - hosts: local
      roles:
        - role: git_code_pull
          code_repo: "ssh://git@dev.goclean.catzcode.com:2222/nerdsville/goclean.git"
          code_root: "/home/code/goclean/branches"
          current_branch: "dev"
