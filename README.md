# API Testing on Restful-Booker
- Here is the Base_Url: [https://restful-booker.herokuapp.com](https://restful-booker.herokuapp.com)

### API testing steps :
1. First open the [documentation](https://docs.google.com/document/d/1YyzPMbEu6eEMFrvp-WHiJW-SvDTJvikqx1QGyyFgRXw/edit)

2. Then launch the [Postman software](https://www.postman.com).

3. After that, create a new collection. If you want you can rename it. You can see in the below image.
<img src= "https://github.com/Rakesh6430/API-Testing-On-Restful-Booker/blob/main/API%20SS/Create%20new%20collection.jpg" height = "300" width="600" >

4. Afterwards, if you hover the mouse on the newly created collection, you will see a three doted icon.

5. After clicking on the three doted icon, you will see some options. 

6. Among the options you will have click on the Add request option.

7. After that, you will see a new request has been added. 

8. Now we have to set the request to POST method. For that, we can add new data to the database of that server.

9. From the documentation, we have to copy the "Base_Url/booking/"

10. Then we have to paste it on the "Enter url or paste text" field.

11. After that, we have to click on body. Then set the text in raw and text format to JSON

12. Then we have to copy the data paste it on the JSON Request body. You will see the demonstration in the below image

13. Then click on save and click on the send button.

14. After that, you will receive some data in the JSON Response body. This is how we ensure that, the information we want to add, 
    has been added with a new booking id.

15. To fetch the data from the database of that server, we have to use GET method. For that, we have to create a new add request and 
    set it to GET method.

16. Now we have to copy "Base_Url/booking/id" and paste it on the "Enter url or paste text" field.

17. Then click on the send button. In the JSON response body , you will see the data which was added has been fetched from the server.
    Now we are ensured that, the data has been added successfully.

18. Now we can update some fields of that data also. To do that, we have to create Token to get permission from the API.

19. First we need to create a new request and set it to POST method.

20. From the documentation, we have to copy "Base_Url/auth"

21. Copy the data which is under the Example field and paste it on the JSON response body.

22. Click on send button. You will get a new token in the JSON reponse body which was sent by the API.

23. The create a new request and SET it to PUT method. Paste the "Base_Url/booking/id" on the field. 

24. The go to Headers section. After that, set the key to Cookies and value to token = "generated value". According to the below image.

25. Copy the data and paste it on the request body. Then, change the first name and last name according to the below image.

26. To check the first name and last name of that has been updated or not in the database of that server. We can again use GET method 
    and request API to fetch the data to check. Now you can see the data hase been update in the database of that server in the below 
    image.

