# Secrets

Secrets is a web application that allows users to login and share a "secret" anonymously. Access demo site [here](https://shielded-plateau-16582.herokuapp.com/).

It uses passport.js to authenticate users. Users can register using an email and password or login with Google:

  1) Users login with username (email) and password. The strategy used to authenticate users is [passport-local](http://www.passportjs.org/packages/passport-local/). They use salting and hashing to protect the passwords in the back end.
  2) The second strategy is using a google account for authentication. The app utilizes [passport-google-oauth20](http://www.passportjs.org/packages/passport-google-oauth20/) to achieve authenticaiton.

## Demos

##### User register/login using passport-local:
<img src="https://github.com/akhan445/Authentication-Secrets/blob/master/register-user.gif" width="auto" height="500" />

##### User register/login with Google:
<img src="https://github.com/akhan445/Authentication-Secrets/blob/master/google-login.gif" width="auto" height="500" />

- Screenshot of database. Shows the google user and locally registered user. Local user is protected using salting and hashing.
    <img src="https://github.com/akhan445/Authentication-Secrets/blob/master/backend-password.png" width="auto" height="400" />

    
##### Submit secret:    
<img src="https://github.com/akhan445/Authentication-Secrets/blob/master/submit-secret.gif" width="auto" height="500" />

##### Edit secret:  
- User is only allowed to have one secret. Editting or trying to add a new secret will replace previous secret.
<img src="https://github.com/akhan445/Authentication-Secrets/blob/master/edit-secret.gif" width="auto" height="500" />
