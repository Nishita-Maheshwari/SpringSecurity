# SpringSecurity

# => NOTE :-
 We can achieve security in J2EE technologies i.e. JSP & Servlets, but it was difficult to implement the security and was also limited.

# => Spring Security :-
	-> History :-
		= Earlier spring security was only the project which was started in 2003 by Ben Alex
		= Then in 2004, it was publicly released under Apache Licence
		= Then in 2008, it was publicly release by new name i.e, Spring Security 2.0.0
		= Now Spring Security is a "framework"
		
# 	-> Advantages :-
		= Open source lightweight framework
		= Highly strong and plugable framework
		= Supports java configuration
		= Can be integrated with Servlet API, Spring MVC and many other technologies
		= Protects against important attacks (session fixation, clickjacking etc) and other common attacks (Brute Force, CSRF, XSS, MITM etc)
		
# 	-> Types of Spring Security (Spring Security Features) :-
		= HTTP Basic Authentication
		= HTTP Digest Authentication
		= Form Based Authentication
		= LDAP (Lightweight Directory Access Protocol) Authentication
		= JAAS (Java Authentication and Authorization Service)
		= Open Id Authentication
		= Remember-me Authentication
		= In-memory Authentication
		= API Security with JWT (JSON Web Tokens)
		= OAuth 2.0
		  etc
	-> NOTE : Spring security mostly focus on 2 main areas i.e. "Authentication" and "Authorization"
# 		= Authentication :-
			- It is the first level check where the user identity is verified who is trying to access a particular resource
			- There are 2 types of authentication :-
				1. Knowledge based authentication
					* username and password
					* pincode
					* providing answer to personal question
				2. Possession based authentication
					* Phone or text messages
					* Key cards and badges
					* Access token device
# 		= Authorization :-
			- It is the process of providing special permissions or authority or actions to a particular user in the application
			
# 	-> Flow of Spring Security :-

![image](https://github.com/Nishita-Maheshwari/SpringSecurity/assets/47790697/453d9619-b0d6-4490-aa90-1f8a954bf5fd)





# => Difference between "HTTP Basic Authentication" and "HTTP Digest Authentication"
	-> Basic :-
		= Basic Authentication uses base64 encoding (not encryption) for genrating our cryptographic string which contains the information of username and password
		= It is easier to implement
	-> Digest :-
		= Digest Authentication uses the hashing (digest means cut into small parts) mechanism for genrating our cryptographic string which contains the information of username and password
		= It is complex to implement
		
# => CSRF :-
	= Full form of CSRF is "Cross-Site Request Forgery" (sometimes it is also known as XSRF)
	= It is an attack that can trick an end-user using a web-application to unknowningly execure actions that can compromise security
	= To overcome this attack, we should include an input hidden to send the CSRF token in the POST method when the user submits the form :-
		
		
