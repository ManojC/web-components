## Web Component For Login ##
This custom element provides a functionality of a login widget & it comes up with following features.

 - **Header Attribute**
	
	> This attribute is used to change the header.
	> It's default value is `Login`
	> 
	> Example -
	> `<t-login-widget header="Sign In"></t-login-widget>`
	> 
	> ![manoj](http://imageresize.org/Output/83363289-5ee1-43b0-8ff6-4b5693e1c16d.jpg)
	
 - **Post Url Attribute**
	
	> Upon setting this attribute with a valid post url, this component will fire a post call to this url.
	The response data from post call is made available using a custom event **`login-success`**.
	If the post url attribute is not set, **`login-success`** event is fired without making the post call.
	The payload for this post call is an object like -
  
  > `{
      username: 'John Doe',
	    password: 'qwerty123!@#'
    }`
    
	> Example -
	> `<t-login-widget post-url="/login"></t-login-widget>`
