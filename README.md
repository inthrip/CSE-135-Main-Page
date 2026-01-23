# CSE-135-Main-Page

## Team Members
- Derrick Burton (Alone)
## Grader Access Info
- Grader Username: grader
- Grader Droplet User Password: kuteY!74o
- Grader htpassword: copiCt9pios
## Site Link
- https://tunkd.com
## Github Auto Deploy Setup
Created a new GitHub repository, copied and added all the relevant files and relevant directories. Created and authorized SSH key in droplet for GitHub deploying. Added three GitHub Secrets to the repository, DEPLOY_HOST (droplet IP), DEPLOY_USER (derrick, my user on droplet), and DEPLOY_KEY(private SSH key). Then added a GitHub Actions workflow .github/workflows/deploy.yml using the secrets to deploy to droplet on push.
## Username/Password
- My Username: derrick
- My Droplet User Password: urB1s4la$c
- My htpassword: baRotru3s
## HTML File Changes After Compression
After my enabling of Apache mod_deflate, DevTools showed that the responses were compressed. The HTML response in DevTools now show 
Content-Encoding: gzip, Vary: Accept-Encoding, and a reduced Content-Length.
## Removing Server Header
I first installed and enabled ModSecurity, then created a custom conf for server headers, and edited it to set SecServerSignature "CSE 135 Server". After enabling it, Apache responses display this custom Server header instead of the default.
