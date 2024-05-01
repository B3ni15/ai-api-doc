<center>
  <h1>AI API Document</h1>
</center>

Note: This ai is based on chatgpt 3.5, it is also used in huntools. (Please don't spam it too much because it is not certain that it will work.) If you encounter such an error, please let me know! 

## https://ai.devbeni.tech/api/newChat?prompt=(Text)

Note: Here you can create a new chat and write in the **prompt** what you want to ask them!

If **successful**: 

```json
  {
    "status":200,
    "message":"Chat created successfully",
    "time":6000,
    "id":"a913d1e1e58660994c9b2b9ee7501d30"
  }
```

- Status: The status code in this case is 200 (Successful)
- Message: The response message from the API is how it was successful or what just happened.
- Time: The time is about how long it takes to retrieve it! (Not sure if this is just a tip)
- Id: The ChatId is what you need to retrieve the message.

## https://ai.devbeni.tech/api/getChat?id=(ChatId)

Note: From here you can retrieve the AI's answer based on the id.

If **successful**: 

```json
  {
    "status":200,
    "message":"Chat fetched successfully",
    "id":"a913d1e1e58660994c9b2b9ee7501d30",
    "chat":" Szia! Hogyan segíthetek ma?"
  }
```

- Status: The status code in this case is 200 (Successful)
- Message: The response message from the API is how it was successful or what just happened.
- Id: The ChatId is what you need to retrieve the message.
- Chat: The message from the AI ​​(So its answer.)

P.S: If you have retrieved the message again, you will not be able to, it will return this answer:

```json
  {
    "status":404,
    "message":"Chat not found"
  }
```

Thanks for using this ❤️. Share it or give it a star, it would help a lot 😀





