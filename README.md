# Write Message
POST http://localhost:8000/api/messages/

body: 
{
  "sender": 1,
  "receiver": 1,
  "subject": "subject example",
  "message": "message example"
}

# Get all messages for a specific user 
GET http://localhost:8000/api/users/<user_id>/messages/

# Get all unread messages for a specific user
GET http://localhost:8000/api/users/<user_id>/messages/?seen=False

# Read message (return one message)
GET http://localhost:8000/api/messages/<message_id>/

# Delete message (as owner or as receiver)
DELETE http://localhost:8000/api/messages/<message_id>/

# Login url
POST http://localhost:8000/api/accounts/login/

{
  "username": "username",
  "password": "password"
}

# logout url
POST http://localhost:8000/api/accounts/logout/

