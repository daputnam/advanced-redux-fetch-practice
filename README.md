### Setup
* Fork, Clone, yarn install, yarn start
* Do Not use the instructions as your guide for what code to type, use the reference guide project (address book)

### Use local api
* http://localhost:4001/products
* http://localhost:4001/contacts
* http://localhost:4001/vehicles
* http://localhost:4001/comments


### Create actions in actions/index.js to retrieve data
*x loadContacts
    * return a thunk function
    * make a fetch call to /contacts
    * in the second then, dispatch to contactsLoaded
*x contactsLoaded(contacts)
    * return an action
    * type is “CONTACTS_LOADED”
    * value is contacts
*x loadVehicles
    * return a thunk function
    * make a fetch call to /vehicles
    * in the second then, dispatch to vehiclesLoaded
*x vehiclesLoaded(vehicles)
    * return an action
    * type is “VEHICLES_LOADED”
    * value is vehicles
*x loadComments
    * return a thunk function
    * make a fetch call to /comments
    * in the second then, dispatch to commentsLoaded
*x commentsLoaded(comments)
    * return an action
    * type is “COMMENTS_LOADED”
    * value is comments
*x loadProducts
    * return a thunk function
    * make a fetch call to /products
    * in the second then, dispatch to productsLoaded
*x productsLoaded(products)
    * return an action
    * type is “PRODUCTS_LOADED”
    * value is products

### Create actions in actions/index.js to create data
*x createProduct(product)
   * return a thunk function
   * make a fetch call to /products as a POST
   * include the product in the body 
   * in the first then, dispatch to loadProducts

*x createContact(contact)
   * return a thunk function
   * make a fetch call to /contacts as a POST
   * include the contact in the body 
   * in the first then, dispatch to loadContacts

*x createComment(comment)
   * return a thunk function
   * make a fetch call to /comments as a POST
   * include the comment in the body 
   * in the first then, dispatch to loadComments

*x createVehicle(vehicle)
   * return a thunk function
   * make a fetch call to /vehicles as a POST
   * include the vehicle in the body 
   * in the first then, dispatch to loadVehicles

### Create reducers in reducers/index.js
*x Create reducers based on the state in state.js
*x Determine which action the reducers should care about 
*x return the appropriate value

### AppContainer
*x In AppContainer.js
*x Import connect
*x Import actions loadContacts, loadVehicles, loadComments, loadProducts
*x mapDispatchToProps for these actions to props of the same name
*x Connect and export
*x Remember how to use connect when there is no mapStateToProps

### App
*x In App.js
*x call loadContacts, loadVehicles,loadComments,loadProducts in componentDidMount

### Points
* Base points - 20
* Contacts appear in list - 10
* Vehicles appear in list - 10
* Comments appear in list - 10
* Products appear in list - 10
* Create new contact shows up in list - 10
* Create new vehicle shows up in list - 10
* Create new comment shows up in list - 10
* Create new product shows up in list - 10



