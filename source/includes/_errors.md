# Errors

LIM API uses the following error codes:


Error Code | Meaning
---------- | -------
400 | Bad Request -- Your request sucks
401 | Unauthorized -- Your API key is wrong
404 | Not Found -- The specified user could not be found
405 | Method Not Allowed -- You tried to access a user with an invalid method
406 | Not Acceptable -- You requested a format that isn't json
410 | Gone -- The user requested has been removed from our servers
422 | Unprocessable Entity -- Backend validation erros
500 | Internal Server Error -- We had a problem with our server. Try again later.
503 | Service Unavailable -- We're temporarily offline for maintenance. Please try again later.
