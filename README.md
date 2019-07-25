# React-Redux-Firebase-Boilerplate
 
#### Author: [Whitney Griffith - ImpactWhit](https://www.linkedin.com/in/whitneygriffith/)


## Built from: 
React-Redux-Firebase-Router [Tutorial1](https://dusty.phillips.codes/2018/08/25/react-redux-firebase-with-firestore-tutorial/)
[Tutorial2](https://medium.com/quick-code/how-to-integrate-react-redux-and-firebase-in-3-simple-steps-c44804a6af38)
[Tutorial3](https://medium.com/quick-code/adding-authentication-to-react-redux-firebase-app-f0efcb1c519a)


[UI Builder - Sketch & Pagedraw](https://pagedraw.io/)


## Instructions

### Starting the project
* ```git clone https://github.com/whitneygriffith/react-redux-firebase```
* create ```src/config/dev.js```in main folder and populate it with your personal configs from [Firebase](https://firebase.google.com/) in the following format:

```
export const FirebaseConfig = {
    apiKey: "AIzaSyBnVQDfjkBkZfC7FcqsTpn8o7of45trmqs",
    authDomain: "",
    databaseURL: "",
    projectId: "",
    storageBucket: "",
    messagingSenderId: ""
};
```
* ```npm install```
* ```npm start```

### Adding a new page
Edit the following:
- [App.js](../src/App.js)
    - Import the new page ```import NewPageComponentName from "./components/PageComponentFolder";```
    - Within the ```<div>``` tag embedded in ```<BrowserRouter>``` tag, add the following ```<Route exact path="/new_page_url" component={NewPageComponentName} />```
To require Authentication to view a page: 
- [App.js](../src/App.js)
    - Within the ```<div>``` tag embedded in ```<BrowserRouter>``` tag, add the following ```<Route exact path="/new_page_url" component={requireAuth(NewPageComponentName)} />```


### Firebase Additional Suggestions
[ ] Implement Firebase Sign In With Link CallBack using onAuthStateChanged Listener

[ ] Error Handling to display error to user from Firebase's Sign In, Sign Up and other function calls


### Sign Up Additional Suggestions
[ ] Create input pattern validators for Email, Phone Number [Ref](https://www.w3schools.com/html/html_form_attributes.asp)


## Production TODOs

### General
[ ] Separate Client from server side

### Environment Variables
[ ] Set ```env``` to ```production``` in ```config.js```

### Firebase Console
[ ] [Add domain to list of authorized domains](https://console.firebase.google.com/u/1/project/seampay-1d1a9/authentication/providers) 
[ ] [Define what occurs to email action links on android or ios device](https://firebase.google.com/docs/auth/web/passing-state-in-email-actions#configuring_firebase_dynamic_links) 


## References

### React 
[cra-boilerplate](https://github.com/mohandere/cra-boilerplate)

[React + Ecosystem](https://github.com/rwieruch?tab=repositories)


### React + Firebase

[React + Firebase](https://www.robinwieruch.de/complete-firebase-authentication-react-tutorial/)
- [Codebase](https://github.com/the-road-to-react-with-firebase/react-firebase-authentication/tree/65e6c18fb894b847fed0ab6f9bb042b310cfedc2)

###  React + Redux

[React + Redux for Beginners](https://www.valentinog.com/blog/react-redux-tutorial-beginners/)

[Getting Started with Redux](https://egghead.io/courses/getting-started-with-redux)

[Taming the state with React](https://roadtoreact.com/course-details?courseId=TAMING_THE_STATE)

[React 101 ](https://tighten.co/blog/react-101-part-4-firebase)

[React Redux Tutorial for Beginners: The Definitive Guide (2018)](https://www.valentinog.com/blog/react-redux-tutorial-beginners/#React_Redux_tutorial_connecting_React_with_Redux)

### React + Redux + Firebase
[React + Redux + Firebase](http://react-redux-firebase.com/)

[Tutorial for React + Firebase + Redux Codebase](https://github.com/wickard/redux-firebase-tutorial)

[How to Integrate React Redux and Firebase in 3 Simple Steps](https://medium.com/quick-code/how-to-integrate-react-redux-and-firebase-in-3-simple-steps-c44804a6af38)

[react-redux-firestore-boilerplate](https://github.com/rioam2/react-redux-firestore-boilerplate)

[Firebase login with email, Fb, Twitter, Google or Github](https://github.com/polinazolotukhina/Social-login)

[generator-react-firebase](https://github.com/prescottprue/generator-react-firebase)


### Firebase

[Email Link Authentication](https://firebase.google.com/docs/auth/web/email-link-auth)

[Email Link Authentication Code Example](https://github.com/firebase/quickstart-js/blob/master/auth/email-link.html#L89)

[Email Link Authentication Repos](https://github.com/search?o=desc&p=2&q=signinwithemaillink&s=indexed&type=Code)

## React + NodeJs Backend

[Connecting ReactJS Frontend with NodeJs Backend](https://www.zeolearn.com/magazine/connecting-reactjs-frontend-with-nodejs-backend)
