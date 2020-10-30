### 1. Sign up
- onClickSignButton:   
call backend sign up api and make a new user. If successful, redirect to main page.

### 2. Log In
- onClickLoginButton:   
call backend sign in api. If authenticated successfully, change state accordingly and redirect to main page. If not, alert!

### 3. Create Page
* onClickCreateSubmitButton:   
Create a new recipe. Send create-recipe data to server to update the server database. Redirect to newly created recipe page.
* onClickAddstepButton:  
Add a new step in Create Page. New Description(Text) and Image field created.
* onClickCreateIngredientSelect:   
Search the typed ingredient in the server database and show the result. The user select the ingredient shown.

### 4. Main Page
* onClickRandomRecipeImage:   
In main page, we show daily random recipe for users. If user click the image/division, redirect to corresponding recipe detail page.
* onClickCreateRecipeImage:   
Redirect to create recipe page.
* onClickRandomRecipeImage:   
In main page, we show recommended recipe for users. If user click the image/division, redirect to corresponding recipe detail page.

### 5. 
