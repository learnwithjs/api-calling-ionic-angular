This is an ionic app.
I have created this application because i want to know that how i can make api calling in ionic angular with the help of services.

Also i want to know that

- what is the role of correct path,
- what is the params in path,
- how to add api key in url,
- how to add a uri in path,
- how to design frontend of app by using ionic angular component
- how to generate service and page by using ionic g page/ service "page-or-service-name"
- what is the role of constructor in class
- where to define method in class
- where and how to declare variables in class

Introduction of this application: --

this is an application in which you can search the details of any movie.
As you can see that in the first page of this application, there is a search bar, where you type the name of any movie, or series or episode.
and also you can select the type of the thing which you want to see.

How this app works?

where any user enter any name in search bar, then this name goes in search term, and it call searchChanged(event) which is defined in movies.page.ts.

in searchChanged($event) method, we call the method searchData(this.searchTerm, this.type) of movie.service.ts.

searchData(this.searchTerm, this.type), in this method we call an api with get request.

in movie.service.ts page, we have added our own api key which we got by signing on 'http://www.omdbapi.com/' website.
and after entering details, we get an email to verify our api key, and in that mail, we also get our api key.

we can add that api key in our path of url.

getDetails(id) function help us to get the information of particular movie by calling api, and it sends the information to the frontend of application, and after that we can see the information in our user screen.

we imported HttpClient in movie.service.ts, by which we can make http request
