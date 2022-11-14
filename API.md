BASE URL: 
URI
ENDPOINT URL : https://github.com/


1. I will create one repository   ----Create ----- POST

  curl \
  -X POST \
  -H "Accept: application/vnd.github+json" \ 
  -H "Authorization: token <TOKEN>" \
  
  token: ghp<>Token
  
https://api.github.com/orgs/ORG/repos 
\
  -d '{"name":"Hello-World","description":"This is your first repository","homepage":"https://github.com","private":false,"has_issues":true,"has_projects":true,"has_wiki":true}'


END POINT: https://api.github.com/orgs/automation-en/repos 
   Http: Post
   -H "Accept: application/vnd.github+json" \ 
   Content-Type : application/json
   -H "Authorization: token <TOKEN>" \

   Payload:
   {
    "name": "Rest4",
    "description": "This is Myfirst RESt3 first repository",
    "homepage": "https://github.com",
    "private": false,
    "has_issues": true,
    "has_projects": true,
    "has_wiki": true,
    "allow_squash_merge" : true
}

2. I will get repository info     ----Read ------- GET

   https://api.github.com/repos/shabbi123/Andriod
    Http: Post
    -H "Accept: application/vnd.github+json" \ 
   Content-Type : application/json
   -H "Authorization: token <TOKEN>" \

   curl \
    -H "Accept: application/vnd.github+json" \ 
    -H "Authorization: token <TOKEN>" \


Responce
:

3. Update repository              ----edit-------- PUT PATCH 
https://github.com/automation-eng/Rest4
    "description": "This is Myfirst RESt4 updated repository",
    "homepage": "https://github.com", with "https://google.com"

    Payload:
     {
    "name": "Rest4",
    "description": "This is Myfirst RESt4 updated repository",
    "homepage": "https://google.com",
    "private": false,
    "has_issues": true,
    "has_projects": true,
    "has_wiki": true,
    "allow_squash_merge" : true
    }


4. Delete Repository              --Deletion ----- DELETE

  curl \
  -X DELETE \
  -H "Accept: application/vnd.github+json" \ 
  -H "Authorization: token <TOKEN>" \
https://api.github.com/repos/OWNER/REPO


  END point URL to delete repo

https://api.github.com/repos/automation-eng/Rest4

  Http: DELETE
https://api.github.com/repos/automation-eng/Rest4




