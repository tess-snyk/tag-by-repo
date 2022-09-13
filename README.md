snyk.io free trial - upgrade to Business or Enterprise to get API access

Import a project: https://docs.snyk.io/integrations/git-repository-scm-integrations/github-integration

Fork this to see some vulns: https://github.com/tess-snyk/juice-shop

1. Dataset containing tag (repo) names:

bitbucket-cloud-import-targets.json

example:
{
  "targets": [
    {
      "target": {
        "owner": "tess-davis",
        "name": "tag-demo-service-1",
        "branch": "main"
      },
      "integrationId": "xxxx",
      "orgId": "90b42513-faa5-4085-a5d4-09c52bd65dfb"
    }
  ]
}

2. For each OrgID in 1. iterate through:

https://snyk.docs.apiary.io/#reference/projects/all-projects/list-all-projects

Send output to become dataset containing project ID and "projects" name:

{
  "org": {
    "name": "defaultOrg",
    "id": "689ce7f9-7943-4a71-b704-2ba575f01089"
  },
  "projects": [
    {
      "name": "atokeneduser/goof",
      "id": "6d5813be-7e6d-4ab8-80c2-1e3e2a454545",
      
      ........


3. Example format tag tool compatible:


