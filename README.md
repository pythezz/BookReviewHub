Book Review Hub:

Book Review Hub is a web application for managing books and their genres. Users can view, create, edit, and delete books and genres, as well as give them ratings. In phase 2(asp.net advanced module) the users will be able to post reviews of the books. The project is built with ASP.NET Core MVC, Entity Framework Core, and Bootstrap for responsive design.

Features:

- Full CRUD operations for Books

- Full CRUD operations for Genres

- Server-side and client-side validation for all forms

- Navigation links for all main pages (Home, Books, Genres)

- Responsive UI using Bootstrap

(Reviews model is included but functionality will be implemented in phase 2.)

Technologies Used

- ASP.NET Core 6

- Entity Framework Core

- SQL Server / LocalDB

- Bootstrap 5

- C# 10

- Razor Pages / MVC

Setup Instructions:
- Clone repository
  git clone https://github.com/pythezz/BookReviewHub
  cd BookReviewHub
  
- Restore NuGet packages
  dotnet restore

- Apply database migrations
  dotnet ef database update

- Run project
  dotnet run

- Open localhost
  http://localhost:5024/


Project uses local database with trusted connections. No credentials required

"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=BookReviewHubDb;Trusted_Connection=True;MultipleActiveResultSets=true"
}
No additional environment variables or API keys are required for local testing.

Default data:
Upon running the project, there will be initial genre data seeded. There will be no books - you need to add one yourself. After adding a book, you will not be allowed to delete the genre attached to it.
- Fiction
- Non-Fiction
- Science Fiction
- Fantasy
- Mystery
- History
- Biography
- Self-Help
- Romance
- Thriller

Views:
Home Page – landing page with links to Books and Genres
Books Index – lists all books with Edit, Details, and Delete options
Books Create/Edit – forms for managing books, including selecting a genre
Books Details - shows details for selected book
Genres Index – lists all genres with Edit, Details, and Delete options
Genre Details - shows details for selected genre
Genre Create/Edit – forms for managing genres
