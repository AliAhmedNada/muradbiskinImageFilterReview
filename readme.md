## Code Review for Image Filter Project 

### So far so good, you're almost there , you might need to do some work to finish this project , Don't Stop , Keep learning with Udacity 💪💪💪💪💪 


#### Engineering Process and Quality
❏ All project code is stored in a GitHub repository and this link has been submitted
for review. There are at least two branches - one for development (dev,
development) and one master. Master should contain the most up-to-date, stable
code at the time of submission.
```
❌this part isnt satisfied as repo was deleted or missing 
"https://github.com/muradbiskin/udacity-cloud-developer-project-2"
try to push your code to the repo again and create master and dev branch to the repo and make sure to be public
```
<img src="https://github.com/AliAhmedNada/muradbiskinImageFilterReview/blob/master/images/repo%20not%20found.PNG" alt="image posted" width="250"/> <br>


❏ Any variables use typescript typing wherever possible, variable and function
names are clear, endpoints are logically named. Good coding practices are
followed.
```
✔️	you satisfied this part but you might need more enhancements, always define types of variables .
💡   example `app.get( "/", async ( req: any, res: any )`
```
#### Development Server
❏ Starting the server with npm run dev runs a local instance of the server with no
errors
```
✔️ this part is working properly with no issues 
```
❏ The stubbed @TODO1 endpoint in src/server.ts is completed and accepts
valid requests including:
http://localhost:{{PORT}}/filteredimage?image_url=https://timedotcom.files.wordpr
ess.com/2019/03/kitten-report.jpg
```
✔️ current image is corrupted and missing , i've used another image , it worked perfectly ..
```
<img src="https://github.com/AliAhmedNada/muradbiskinImageFilterReview/blob/master/images/Capture.PNG" alt="image posted" width="250"/>

❏ Successful responses have a 200 code, at least one error code for caught errors
(i.e. 422) <br>
```
❌	 for wrong urls it didnt work as expected ,response status return is 404 not 422 
```
<img src="https://github.com/AliAhmedNada/muradbiskinImageFilterReview/blob/master/images/404.PNG" alt="image posted" width="250"/>
<br>

💡Always use try and catch in your code as it is the best pratice to handle errors that is unexpected use it in utils/utils.ts and server.ts


```
example
server.ts
try {
    res.sendFile(response);
} catch (err) {
    res.status(422).send("Please send the correct image_url");
}
utils.ts
   return new Promise(async resolve => {
        try {
   /*the code of the utils */
        } catch (err) {
            resolve(err.message)
        }
```

#### Elastic Beanstalk Deployment
❏ An endpoint URL for a running elastic beanstalk deployment (EB_URL) has been
submitted along with the project submission. This endpoint responds to valid
GET requests including:
http://{{EB_URL}}/filteredimage?image_url=https://timedotcom.files.wordpress.co
m/2019/03/kitten-report.jpg
```
❌ the elastic bean APP is not working nor responding , it seems it is off or deleted please start it again 
```
<img src="https://github.com/AliAhmedNada/muradbiskinImageFilterReview/blob/master/images/beanelastic.PNG" alt="image posted" width="250"/>
http://udacity-cloud-developer-project-2.eu-central-1.elasticbeanstalk.com/
<br>

❏ The project was deployed using the AWS Elastic Beanstalk CLI eb init, eb
create, and eb deploy commands.
A screenshot of the elastic beanstalk application dashboard is included in a
deployment_screenshot directory.
```
✔️ this requirement is satisfied from screenshot attached 
```
<img src="https://github.com/AliAhmedNada/muradbiskinImageFilterReview/blob/master/muradbiskin-udacity-cloud-developer-project-2-5ee970c/deployment_screenshots/deployment_screenshot.png" alt="image posted" width="250"/>

