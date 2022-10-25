# 



## ✨ Code-base structure

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |    |-- paginator.html       # Paginator for bulletin
   |         |
   |         |-- layouts/                     # Master pages
   |         |    |-- base-fullscreen.html    # Used by Authentication pages
   |         |    |-- base.html               # Used by common pages
   |         |
   |         |-- accounts/                    # Authentication pages
   |         |    |-- login.html              # Login page
   |         |    |-- register.html           # Register page
   |         |    |-- policy-check.html       # Policy page for register 
   |         |    |-- policy.html             # Policy page 
   |         |    |-- copyright.html          # Copyright page 
   |         |
   |         |-- home/                        # Actual pages
   |              |-- home.html               # Home page
   |              |-- search.html             # Searching for heritage page
   |              |-- route-bulletin.html     # Route bulletin
   |              |-- route-view.html         # Route post
   |              |-- route-write.html        # Writing route post
   |              |-- route-write-search.html # Searching for heritage on route post
   |              |-- support-bulletin.html   # Support bulletin
   |              |-- support-view.html       # Support post
   |              |-- support-write.html      # Writing question post
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />