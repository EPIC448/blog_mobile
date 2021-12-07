 <!--  Focus on this app is to see how data flow through the application -->
 <!--  Completed so far 
  installed 
  "npm install react-navigation"
   -->

   Steps I was following. and Internet off line.

    Issues with Current React code. [Resolved]
    https://github.com/facebook/react-native/issues/27029


 Header Deprecation message. Use the code below inside. 
  return {
    headerRight: () => (
      <TouchableOpacity onPress={() => navigation.navigate('Create')}>
        <Feather name="plus" size={30} />
      </TouchableOpacity>
    ),
  };

  Note: the EDit Icon is not showing on my page yet. 


  <!--  Started to write this from the Video of  =>>> Data API Sync --> title Outside Data API

  Used Json Server. 
   We use ngrok Server which we create in another Directory outside of the BLOG_MOBILE.
 Install JSON- 
  npm install json-server ngrok

  New Setup Json Server in Ngrok. 
  got to Ngrok Directory in another file to make this possible. 

  After you down with following the steps from the JsonServer located in an Outside folder. 

Note: making call to the jsonServer will note work if you dont starte it there first. (because of Ngraka)


  AXIOS
  we install axios.
  We make out request using Method -> get, put etc. 

   Need App FLOW Digram for making request.

  
create the API file, but confiuge it to the endpoint of jsonServer..
 And we added a function "getBlogPosts" in the BlogContext.js  so we can use later.


 Challenge -> Axios Not working. Error.
        Unable to resolve module axios from /Users/codehouse/Documents/Clone_repos/javascript/blog_mobile/src/api/jsonServer.js: axios could not be found within the project.

If you are sure the module exists, try these steps:
 1. Clear watchman watches: watchman watch-del-all
 2. Delete node_modules and run yarn install
 3. Reset Metro's cache: yarn start --reset-cache
 4. Remove the cache: rm -rf /tmp/metro-*
> 1 | import axios from 'axios';
    |                    ^