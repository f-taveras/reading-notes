<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

# What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?

Key Components and Purpose:

* __Purpose:__ DRF permissions are used to grant or deny access to different parts of your API based on the request method and user authentication status. They play a crucial role in securing your API by ensuring that only authorized users can perform certain actions.
* __Key Components:__
    - Permission Classes: These are Python classes that define the permission logic. The most common ones include AllowAny, IsAuthenticated, IsAdminUser, IsAuthenticatedOrReadOnly, and custom permission classes that you can define as needed.
    -Permission Policies: These are applied globally or at a view level. Global permissions are defined in the DRF settings (DEFAULT_PERMISSION_CLASSES), while view-level permissions are set by adding the permission_classes attribute to your view.
* __How They Help in Securing an API:__
    - __Granular Access Control:__ Permissions allow for fine-grained control over who can access your API endpoints, ensuring that users can only perform actions they are authorized for.
    - __Protection Against Unauthorized Access:__ By default, DRF will deny access to any part of the API that hasn't explicitly granted permission, providing a secure default stance.
    - __Customizable:__ DRF's permissions system is highly customizable, allowing developers to define complex permission schemes that fit their application's specific needs.

# In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?

Purpose:

The `SELECT` statement in SQL is used to query or retrieve data from one or more tables in a database. It allows you to specify exactly which data you want to fetch, including filtering, ordering, and grouping the results.

__Example:__

* To retrieve all columns from a table called employees, you would use the following SQL query:

```
SELECT * FROM employees;
```
* In this statement, `*` represents all columns, and employees is the name of the table from which data is being retrieved.

# Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

Role:

* __Simplification and DRY:__ Django Rest Framework's generic views are designed to simplify the development of API endpoints by providing common patterns for CRUD (Create, Read, Update, Delete) operations, thereby adhering to the DRY (Don't Repeat Yourself) principle.

* __Built-in Functionality:__ These views come with a lot of built-in functionality, such as serialization, query handling, and permissions, making it easier and quicker to build RESTful APIs.

Examples of Usage:

* __ListAPIView:__ For listing a queryset or showing all instances of a model. For example, to show all employees in an `Employee` model:

```
from rest_framework.generics import ListAPIView
from .models import Employee
from .serializers import EmployeeSerializer

class EmployeeList(ListAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer
```
* __RetrieveAPIView:__ For retrieving a single model instance. For example, to get a specific employee by their ID:

from rest_framework.generics import RetrieveAPIView

```
class EmployeeDetail(RetrieveAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer
```

* __CreateAPIView, UpdateAPIView, DestroyAPIView:__ Respectively used for creating, updating, and deleting instances. These can be used separately or combined using `ListCreateAPIView` or `RetrieveUpdateDestroyAPIView` for more comprehensive viewsets that handle multiple actions in a single class.

DRF's generic views significantly reduce the amount of code you need to write for standard API functionality, enabling more focus on developing your application's unique features

<sub>Information modeled using ChatGPT</sub>
