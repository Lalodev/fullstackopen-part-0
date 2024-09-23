Exercise 0.4

graph TD;
    A[User writes a note] --> B[User clicks button 'save'];
    B --> C{Empty field?};
    C -->|Yes| D[Ask for information once again, except empty];
    C -->|No| E[Send new_note to Server using POST verb];
    E --> F[Server receives the new_note and validate it? ];
	F -->|Yes| G[Show the exception error];
    F -->|No| H[Save the new_note];
	H --> I[Show the success message];
    I --> J[The browser receives the anwser];
    J --> K[The browser updates the view];

	
Exercise 0.5

graph TD;
    A[User opens the SPA] --> B[Browser requests all files which are necesary from https://studies.cs.helsinki.fi/exampleapp/spa];
    B --> C{Server sends all files to the browser, HTML, CSS and JS files};
    C --> D{Browser loads all elements on DOM};
	D --> E{Browser shows all information through React};	
	
Exercise 0.6

graph TD;
    A[User writes a note on input field on https://studies.cs.helsinki.fi/exampleapp/new_note] --> B[User clicks button 'save'];
    B --> C{Empty field?};
    C -->|Yes| D[Ask for information once again, except empty;
    C -->|No| E[Send new_note to Server using POST verb on https://studies.cs.helsinki.fi/exampleapp/new_note];
    E --> F[Server receives the new_note and validate it? ];
	F -->|Yes| G[Show the exception error];
    F -->|No| H[Save the new_note];
	H --> I[Show the success message];
    I --> J[The browser receives the anwser ];
    J --> K[The browser updates the view] https://studies.cs.helsinki.fi/exampleapp/notes;