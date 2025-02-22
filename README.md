# Kaminari::Tailwind

kaminari-tailwind is a Ruby gem that provides a Tailwind CSS–based pagination template for Kaminari. With minimal setup, you can quickly get a responsive pagination style in your Rails applications.

## Features

- Seamless integration with Kaminari pagination
- Pre-built pagination views styled with Tailwind CSS
- Easy to customize—simply modify the generated partials to fit your design

## ScreenShot

![ja](docs/img/ja.png)
![en](docs/img/en.png)

## Installation

1. Add the following lines to your Gemfile:

```
gem 'kaminari'
gem 'kaminari-tailwind'
```

2. Run bundle install to install the gems:

`bundle install`

## Getting Started

1. Set up pagination in your controller:

```ruby
def index
  @users = User.page(params[:page]).per(10)
end
```

2. Add pagination links in your view:

```ruby
<%= paginate @users, theme: 'tailwind' %>
```

Here, theme: 'tailwind' tells Kaminari to use the Tailwind-based views provided by this gem.

## Customization

- If you ran rails generate kaminari:views tailwind, you can edit the generated partials in app/views/kaminari/ to change classes, spacing, colors, etc.
- Adjust your tailwind.config.js if you have a custom Tailwind setup or want to add utility classes.

## Contributing

1. Fork this repository and clone it to your local environment.
2. Create a new branch for your feature or bugfix.
3. Make your changes, add tests, and run the test suite (if applicable).
4. Submit a Pull Request.

We appreciate all contributions—bug reports, feature requests, and pull requests are welcome!

## License

This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to add badges, screenshots, or any additional sections (e.g., FAQ, advanced usage) to make your README more comprehensive.
