To run elixir:
> docker-compose run lab

mix new lab
cd lab
mix test

# mix.exs
def deps do
  [
    ...
    {:mix_test_watch, "~> 0.5", only: :dev, runtime: false}
    ...
  ]  
end

# helpers:
Stream.cycle(enumerable): Creates a stream that cycles through the given enumerable, infinitely

Enum.take(enumerable, amount): Takes the first amount items from the enumerable