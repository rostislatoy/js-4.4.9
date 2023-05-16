1. POST запрос на https://blog.kata.academy/api/users

BODY - {
  "user": {
    "username": "Jaden75",
    "email": "jaden75@gmail.com",
    "password": "Pjkjnwt1"
  }
}

2. POST запрос на https://blog.kata.academy/api/users/login

BODY - {
  "user": {
    "email": "jaden75@gmail.com",
    "password": "Pjkjnwt1"
  }
}

RESPONSE - {
    "user": {
        "username": "jaden75",
        "email": "jaden75@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0NjM1OWI2NjBjNjc1MWIwMGI3NzQxMyIsInVzZXJuYW1lIjoiamFkZW43NSIsImV4cCI6MTY4OTQxNjg4MSwiaWF0IjoxNjg0MjMyODgxfQ.X7XMCr6W9K03ENmGVWhXgp9ghySU8QZ2z2VR7HcW9y4"
    }
}

3. GET запрос на https://blog.kata.academy/api/user

HEADERS - 

Autorization   -   Token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0NjM1OWI2NjBjNjc1MWIwMGI3NzQxMyIsInVzZXJuYW1lIjoiamFkZW43NSIsImV4cCI6MTY4OTQxNjg4MSwiaWF0IjoxNjg0MjMyODgxfQ.X7XMCr6W9K03ENmGVWhXgp9ghySU8QZ2z2VR7HcW9y4

REPSPONSE - {
    "user": {
        "username": "jaden75",
        "email": "jaden75@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0NjM1OWI2NjBjNjc1MWIwMGI3NzQxMyIsInVzZXJuYW1lIjoiamFkZW43NSIsImV4cCI6MTY4OTQxNjkwMywiaWF0IjoxNjg0MjMyOTAzfQ.0jM0c41SCZvacwQqLsPrROWerfVG1HUc2hdIarQVDBg"
    }
}
