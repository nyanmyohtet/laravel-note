# Naming Convention in Laravel

## Naming Controller

Capitalized.

E.g, UserController, etc.

## Database Table

snake_case in plural form.

E.g, users, roles, etc.

## Pivot Table

each model in alphabetical order, separated by underscore (snake_case).

E.g, role_user

## Table Column Name

snake_case.

E.g, post_body, id, created_at, etc.

## Primary Key

normally, `id`

## Foreign Keys

model name(singular) with `_id` append.

E.g, user_id, role_id, etc.

## Variables

camelCase

E.g, $user, $bannedUser, etc.

## Model

singular, no spacing between words and capitalized.

E.g, User, Role, etc.

## Model Properties

snake_case, the same conventions with the table column names

E.g, name, created_at, etc.

## Model Methods

camelCase.

E.g, get(), getAll(), etc.

## Naming for CRUD Operations

| Verb      | URI                | Method    | Route Name    |
| --------- | ------------------ | --------- | ------------- |
| GET       | /posts             | index()   | posts.index   |
| GET       | /posts/create      | create()  | posts.create  |
| POST      | /posts             | store()   | posts.store   |
| GET       | /posts/{post}      | show()    | posts.show    |
| GET       | /posts/{post}/edit | edit()    | posts.edit    |
| PUT/PATCH | /posts/{post}      | update()  | posts.update  |
| DELETE    | /posts/{post}      | destroy() | posts.destroy |

## Traits

Capitalized adjective word.

E.g, Notifiable, Dispatchable, etc.

## Blade Files

snake_case.

E.g, post.blade.php, all_posts.blade.php, etc.
