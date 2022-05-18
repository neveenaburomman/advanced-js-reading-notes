## RBAC
Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for 
advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

## What are cookies in react?
Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that
the users browse and use it to verify them. To set or remove the cookies, we are going to use a third-party dependency of react-cookie.

Install
```ruby
$ npm install react-cookies --save
```
Usage
```ruby 
import { Component } from 'react'
import cookie from 'react-cookies'
 
import LoginPanel from './LoginPanel'
import Dashboard from './Dashboard'
 
class MyApp extends Component {
  constructor () {
    super()
 
    this.onLogin = this.onLogin.bind(this)
    this.onLogout = this.onLogout.bind(this)
  }
 
  componentWillMount() {
    this.state =  { userId: cookie.load('userId') }
  }
 
  onLogin(userId) {
    this.setState({ userId })
    cookie.save('userId', userId, { path: '/' })
  }
 
  onLogout() {
    cookie.remove('userId', { path: '/' })
  }
 
  render() {
    const { userId } = this.state
 
    if (!userId) {
      return <LoginPanel onSuccess={this.onLogin} />
    }
 
    return <Dashboard userId={userId} />
  }
}
```
## How do you add a react cookie?
To set a cookie, we need to import the useCookies() hook from the react-cookie package. The useCookies() hook accepts the array with 
cookie-name as it's first argument and returns the array with two elements cookies object , setCookie() method. The cookies object contains 
all cookies you have created in your app
