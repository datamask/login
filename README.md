# login
http://localhost:8080/oauth2-1.0/oauth/token?grant_type=password&client_id=restapp&client_secret=restapp&username=admin&password=secret

{"access_token":"5e179fde-0bfe-4c8f-9f53-be55deb69453","token_type":"bearer","refresh_token":"a572af98-8c14-4670-8af5-81a8e01d7f7b","expires_in":119}

if no access

<oauth>
<error_description>
An Authentication object was not found in the SecurityContext
</error_description>
<error>unauthorized</error>
</oauth>

if access

7e943d78-0244-43c7-9085-dda7c3bbb18d

http://localhost:8080/oauth2-1.0/api/users/?access_token=11c02495-03df-46d1-8c7b-3c152a176e1f


refresh token

http://localhost:8080/oauth2-1.0/oauth/token?grant_type=refresh_token&client_id=restapp&client_secret=restapp&refresh_token=7e943d78-0244-43c7-9085-dda7c3bbb18d
