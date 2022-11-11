# csrf_app

This is a simple app that allows an authenticated user to create comment and update his username and email address.
After clicking valid_session link on the page user John is logged in and authenticated. After pressing Your page link, John can change his username and/or password. After pressing Save click on link Home to get back to comments section and you can notice that the author of comments is updated accordingly to the user's name. 

### Starting the app
To run this app in one of two modes (vulnerable and safe mode), do the following:
1.  Clone this repository
```shell
git clone https://github.com/Verstopper/csrf_app.git
```

2.  Move inside the repository folder ("root" folder)
```shell
cd .\csrf-app
```

3.  Install dependencies 
```shell  
npm install
```
4. Launch the app in desired mode:

  - Vulnerable Mode: 
  ```shell
  npm run start-vuln
  ```
  
  - Safe mode:
  ```shell
  npm run start-safe
  ```
  
### Testing attack on safe mode and vulnerable mode

To test CSRF attack in either of two modes, launch the app in desired mode and open the app in one tab
and the atttack-server in other tab


[App](http://localhost:3000/) ==> http://localhost:3000/

[Attack-server](http://localhost:4000/) ==> http://localhost:4000/

CSRF attack is implemented in a way that attacker can change user's username and email address.

After clicking on the "Engage attack" link on the attacker's side, refresh app side to see the changes
