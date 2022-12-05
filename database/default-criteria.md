To set default criteria for model operations with Elixir and Ecto, you can use the default_scope/2 macro in your schema module.

Here is an example of how this might work:

```elixir
defmodule MyApp.User do
  use Ecto.Schema

  schema "users" do
    # ...
  end

  @default_scope {where: is_active: true}
end
```

In this example, we have defined a default scope for the MyApp.User schema that will only include users who have the is_active flag set to true.

Once the default scope is defined, it will be automatically applied to all queries performed using this schema. For example:

```elixir

# Only active users will be returned
users = MyApp.User |> Repo.all()

You can also override the default scope in individual queries by using the override_scope/2 function. For example:

# This query will include inactive users as well
users =
  MyApp.User
  |> override_scope(where: is_active: false)
  |> Repo.all()
```

Using default scopes can be useful because it allows you to specify default criteria for model operations, ensuring that your queries always return the results that you expect. It can also make your code more concise and easier to read, since you don't have to specify the same criteria in every query.
