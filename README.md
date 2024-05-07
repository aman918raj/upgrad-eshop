# upgrad-eshop

1. Navigate to frontend folder
2. Run "npm i redux react-redux"
3. Run "npm start" -> will run on localhost:3000
If the above command works, then good else run the below code
npm run build
5. Install mongodb and run it
6. Navigate inside backend folder and run Spring boot App.
7. create products collection inside ecommerce db.
8. Load products collection with json file in the parent project.

NOTE: THERE WAS an ISSUE WITH BACKEND CODE. WE HAVE FIXED BY ADDING BELOW CODE TO BACKED com.upgrad.ecommerce.controllers.AuthController.java FILE. ADDED THE BELOW 3 LINES AFTER LINE NO. 67:
model.put("email", userDetails.getEmail());
model.put("roles", userDetails.getAuthorities().stream().map(GrantedAuthority::getAuthority).collect(Collectors.toList()));
model.put("id", userDetails.getId());
