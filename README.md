# GithubOauth-GO
Use GitHub login on your app.

## How to use it?

1. The first, you can see the function `GetOauthCode(url string)`, the`utils.GitHubID, utils.GitHUbSecret`is your github's id and secret, you should change it. Than you can use the function get an url.
2. Use `GetGitHubToken(url string)`, input your url, you can get user token.
3. Use `GetUserInfo(token string)`, input the token, you can get user information.
4. `CommentToken()` is a middleware if you use gin framework. Sure, you can design your own middleware if you should. The middleware can oauth user by Header's "Authorization".
