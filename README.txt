 architecture de projet :

app
|
| material
   - material.module.ts  //Angular Material elements modules importation 
| Models
   - Product.ts //model de product
   - Utilisateur.ts //model Utilisateur
| Others (sharing components)
  - image-upload //image-upload Component "Child of others Components"
  - navigation  // nav bar Component "Child of app Component "
| Pages 
 -   home (page acceuil Component)
 -  login (login Component)
 -  product-details (product-details component)
 -  profile (profile component)
   signup (signup component)
| Services
  - data-sharing.service.ts (authentification information using BehaviorSubject )
  - products.service.ts  (create and 3 gets with firestore Cloud )
  - user.service.ts ( create,delete, 3 gets with firestore Cloud)

| app-routing (configurate project routes)
| app-component.html(call navigation component and router Outlet )
| app.component.ts
| app.module.ts  (calling different modules used in this project )
|assets
 - css
 -fonts
 -img
|environments  (declare firebase key information)

notes :

- all pages except home and product-details designed with bootstrap the others with angular material 
- ng2searchpipe to filter list displayed in home page 
- add new product with multiple image upload and display with bootstrap carousel


 