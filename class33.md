### **_What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?_***

JSON Web Tokens (JWTs) are used for securely transmitting information between parties. They consist of a header, payload, and signature. The header and payload are JSON objects that are Base64Url encoded. The signature is created by hashing the encoded header, encoded payload, and a secret key. JWTs are used for authentication and authorization purposes in web applications, allowing the server to verify the token's authenticity and extract information from the payload without the need for server-side storage.

### **_How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?_**

To integrate JWT authentication with Django REST Framework (DRF) and secure API endpoints:

Install required packages: Install djangorestframework, djangorestframework-jwt, and pyjwt.

Configure Django settings: Add rest_framework and rest_framework_jwt to INSTALLED_APPS.

Configure JWT settings: Define JWT settings in settings.py like JWT_SECRET_KEY, JWT_ALGORITHM, etc.

Implement authentication views: Create views for token generation and refreshing.

Include JWT URLs: Add JWT authentication URLs to your project's URL configuration.

Secure API endpoints: Use @api_view and @permission_classes decorators to enforce authentication and permissions for each view.

Include JWT authentication: Set DEFAULT_AUTHENTICATION_CLASSES in REST_FRAMEWORK to include JSONWebTokenAuthentication.