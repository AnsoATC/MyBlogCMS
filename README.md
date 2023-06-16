# MyBlog - A Symfony-based Blogging Platform
## Video Demo: https://youtu.be/Nsp9X_VrxM8
## Description:
MyBlog is a powerful and user-friendly blogging platform built with Symfony. It provides an intuitive interface for creating, managing, and publishing blog posts. The platform offers various features such as user registration, authentication, and role-based access control. Users can create and edit blog posts, organize them into categories, and interact with readers through comments. MyBlog also includes a responsive design and SEO optimization for enhanced visibility and user experience.
## Project structure
The project is organized according to the typical structure of a Symfony application. Here is a description of each important file and directory:

**config/** : This directory contains the Symfony application configuration files.

**src/** : This directory contains the Symfony application source code.

**templates/** : This directory contains the template files used to generate the site's views.

**public/**: This directory contains the application's public files, such as images, CSS and JavaScript files.

**bin/** : This directory contains executable scripts for project management.

**vendor/** : This directory contains external project dependencies installed via Composer.

## Important files
### Entity
**Article.php**: Entity class representing an article.

**Category.php**: Entity class representing a category.

**Comment.php**: Entity class representing a comment.

**Media.php**: Entity class representing a media file.

**Menu.php**: Entity class representing a menu item.

**Option.php**: Entity class representing a site option.

**Page.php**: Entity class representing a page.

**User.php**: Entity class representing a user.

### Controller
**ArticleController.php**: Controller for handling article-related functionality on the public site.

**CategoryController.php**: Controller for handling category-related functionality on the public site.

**CommentController.php**: Controller for handling comment-related functionality on the public site.

**HomeController.php**: Controller for the home page of the public site.

**PageController.php**: Controller for handling page-related functionality on the public site.

**UserController.php**: Controller for handling user-related functionality on the public site.

**/Admin**: This directory contains CRUD controllers for managing various entities in the admin dashboard.
**ArticleCrudController.php**: Controller for managing articles in the admin dashboard.

**CategoryCrudController.php**: Controller for managing categories in the admin dashboard.

**CommentCrudController.php**: Controller for managing comments in the admin dashboard.

**DashboardController.php**: Controller for the admin dashboard main page.

**MediaCrudController.php**: Controller for managing media files in the admin dashboard.

**MenuCrudController.php**: Controller for managing menus in the admin dashboard.

**OptionCrudController.php**: Controller for managing site options in the admin dashboard.

**PageCrudController.php**: Controller for managing pages in the admin dashboard.

**UserCrudController.php**: Controller for managing users in the admin dashboard.

### DataFixtures
**OptionFixtures.php**: Fixtures class for populating initial data for site options.

### EventListener
**ExceptionListener.php**: Event listener class for handling exceptions.

### EventSubscriber
**AdminSubscriber.php**: Event subscriber class for admin-related events.

### Form
**/Type**: Directory containing form types for different entities.

**CommentType.php**: Form type for comment entity.

**RegistrationFormType.php**: Form type for user registration.

**WelcomeType.php**: Form type for the welcome section.

### Model
**TimestampedInterface.php**: Interface for entities with timestamped properties.

**WelcomeModel.php**: Model class for handling the welcome section of the site.

### Repository
**ArticleRepository.php**: Repository class for article entity.

**CategoryRepository.php**: Repository class for category entity.

**CommentRepository.php**: Repository class for comment entity.

**MediaRepository.php**: Repository class for media entity.

**MenuRepository.php**: Repository class for menu entity.

**OptionRepository.php**: Repository class for option entity.

**PageRepository.php**: Repository class for page entity.

**UserRepository.php**: Repository class for user entity.

### Service
**ArticleService.php**: Service class for handling article-related operations.

**CommentService.php**: Service class for handling comment-related operations.

**DatabaseService.php**: Service class for interacting with the database.

**MenuService.php**: Service class for handling menu-related operations.

**OptionService.php**: Service class for handling site option-related operations.

### Templates
**base.html.twig**: Base template used as the layout for other templates.
**/article**: Directory containing templates for article-related views.

**item.html.twig**: Template for displaying a single article item.

**list.html.twig**: Template for displaying a list of articles.

**show.html.twig**: Template for displaying the details of an article.

**/category**: Directory containing templates for category-related views.

**show.html.twig**: Template for displaying the details of a category.

**/comment**: Directory containing templates for comment-related views.

**index.html.twig**: Template for displaying comments.

**/home**: Directory containing templates for the home page views.

**index.html.twig**: Template for the home page.

**welcome.html.twig**: Template for the welcome section of the home page.

**/page**: Directory containing templates for page-related views.

**index.html.twig**: Template for displaying pages.

**/user**: Directory containing templates for user-related views.

**index.html.twig**: Template for displaying user profiles.

**login.html.twig**: Template for the user login page.

**register.html.twig**: Template for the user registration page.

**/widget**: Directory containing templates for reusable widgets.

**about.html.twig**: Template for an about section.

**categories.html.twig**: Template for displaying categories as a widget.

## Design choices
When developing this project, I took the following points into account:

**Use of Symfony**: I chose to use the Symfony framework because of its power and flexibility for web application development.

**MVC model**: I followed the MVC (Model-View-Controller) design model to organize the application code and separate business logic from presentation.

**Use of a database**: I used a SQL database to store user profiles. This enables efficient data management and information persistence.

**Security**: I implemented security measures such as user authentication and data validation to prevent attacks and guarantee confidentiality of information.

**Templates and views**: I used Twig template files to generate the site's views. This facilitates the separation of PHP code and HTML presentation.