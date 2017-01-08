#part 1: 3 inital routes
packages: ejs, express


/ : home routes
/camps : list all the camps we have
/camps/new : this creating new camps


skeleton for our project:
public: will host css and js 
    css
    js
views:
    landing.ejs
    camps.ejs
    new.ejs
    partials
    
data and what to display on camps page:

for /camps/new:
form with:
    name
    image
    button
        once user clicked the button /submit the form, it will go to the /camps page and display all the camps along with the newly created one
        NOTE: difference between GET and POST
                GET: to get info from a server
                POST: to add info to the server
        In order for POST to work, we need package:
                body-parser
                    npm install body-parser --save
                    var bodyParser = require("body-parser");
                    app.use(bodyParser.urlencoded({extended:true}));

                    
#part 2: layer and basic styling
1: create header.ejs and footer.ejs in partials folder
2: get bootstrap CDN and put it in header.ejs

jumbotron
grid system
thumbnail
display:flex; flex:wrap:wrap;
form
button
navbar
