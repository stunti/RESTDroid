#change log 0.7.2.5
*	Hotfix: Delete reference to ResourceList class

#change log 0.7.2.4
* Hotfixes : Intent maps is now stored in WebService class not in RestService class. WebService tries to retrieve pending request only if request is GET or DELETE

#change log 0.7.2.3
*	Hotfixes : Remove useless import android.download.Request and rename MainActivity of RESTDroid project

#Change log 0.7.2.2
*	Hotfixes : Removes useless res/ files and 3 seconds test latency in HttpRequestHandler

#Change log 0.7.2.1
*	Hotfix : Set default charset to UTF-8

#Change log 0.7.2
*	Fix bug when dealing with post request (request was not correctly initialized)
*	Fixed bug when calling getResultStream() when request's result stream is null
*	RequestListeners now holds a reference to the RESTRequest wich is holding it
*	Fix bug in Processor.checkRequest when resource's result code is 200 but returns false to not resend the request

#Change log 0.7.1
*	Fix bug with RESTRequest factory in WebService class
*	Result stream send by the server is now accessible within RESTRequest class by calling getResultStream()

#Change log 0.7.0

*	Request listeners now manage with RequestListeners class in order to avoid listener duplication
*	GET/POST/PUT/DELETE methods from WebService class now return instance of RESTRequest already pending or a new instance
*	Request are now executed when you want. Use WebService#executeRequest() from WebService class