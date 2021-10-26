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