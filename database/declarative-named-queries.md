Ecto is a library for Elixir that allows you to create and manage relationships between data in a database. One way to do this is by using named queries, which are pre-defined queries that can be called by name in your code.

To create a named query, you can use the @doc and @spec annotations in your schema module to define the query. Here is an example of how this might look:

```elixir

defmodule MyApp.User do
  use Ecto.Schema

  @doc """
  Get all users who have a given name.

  ## Examples

      iex> MyApp.User.by_name("John")
      [%MyApp.User{name: "John"}, %MyApp.User{name: "John"}]
  """
  @spec by_name(binary) :: [MyApp.User]
  def by_name(name) do
    from u in MyApp.User,
    where: u.name == ^name
  end
end
```

In this example, we have defined a named query called by_name/1 that takes a name as an argument and returns a list of users who have that name. The @doc and @spec annotations provide documentation for the query, explaining what it does and how to use it.

Once the named query is defined, you can call it in your code like this:

```elixir

users = MyApp.User.by_name("John")

```

This will return a list of all users who have the name "John".

Named queries can be useful because they provide a clear and concise way to define common queries that are used throughout your application. They also make it easier to understand and maintain the code, since the queries are defined in a consistent and organized manner.
