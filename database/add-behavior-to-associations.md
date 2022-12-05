In Ecto, you can add behavior to associations by defining custom functions in your schema modules.

Here is an example of how this might work:

```elixir

defmodule MyApp.User do
  use Ecto.Schema

  schema "users" do
    has_many :posts, MyApp.Post
  end

  # Add a custom function to the User schema
  defp favorite_post(user) do
    user
    |> assoc(:posts)
    |> where(title: ^"My Favorite Post")
    |> Repo.one()
  end
end
```

In this example, we have defined a schema for the users table, and added a has_many association with the posts table. We have also defined a custom function called favorite_post/1 that returns the user's favorite post, based on the post's title.

Once the schema and custom function are defined, you can call the function in your code like this:

```elixir

# Get the user's favorite post
user = MyApp.User |> Repo.get(1)
favorite_post = MyApp.User.favorite_post(user)
```

Adding custom functions to associations in your schema can be useful because it allows you to define custom behavior for your data, and to easily reuse that behavior in your code. It can also make your code more readable and maintainable, since the custom behavior is defined in a consistent and organized manner.

Here is an example of a more complicated case where you might want to add behavior to ecto associations:

```elixir

defmodule MyApp.User do
  use Ecto.Schema

  schema "users" do
    has_many :posts, MyApp.Post
    has_many :comments, MyApp.Comment
  end

  # Add a custom function to the User schema
  defp favorite_post(user) do
    user
    |> assoc(:posts)
    |> where(title: ^"My Favorite Post")
    |> Repo.one()
  end

  # Add another custom function to the User schema
  defp most_commented_post(user) do
    user
    |> assoc(:posts)
    |> inner_join(:comments, on: [id: :post_id])
    |> group_by([p], p.id)
    |> order_by([c], desc: count(c.id))
    |> Repo.one()
  end
end
```

In this example, we have defined a schema for the users table, and added has_many associations with the posts and comments tables. We have also defined two custom functions: favorite_post/1 and most_commented_post/1. The favorite_post/1 function returns the user's favorite post, based on the post's title. The most_commented_post/1 function returns the user's most commented post, based on the number of comments on each post.

Once the schema and custom functions are defined, you can call them in your code like this:

```elixir

# Get the user's favorite post
user = MyApp.User |> Repo.get(1)
favorite_post = MyApp.User.favorite_post(user)

# Get the user's most commented post
most_commented_post = MyApp.User.most_commented_post(user)
```

Adding custom functions to associations in your schema can be useful because it allows you to define custom behavior for your data, and to easily reuse that behavior in your code. It can also make your code more readable and maintainable, since the custom behavior is defined in a consistent and organized manner.
