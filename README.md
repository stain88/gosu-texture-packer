# GosuTexturePacker

[![Gem
Version](https://badge.fury.io/rb/gosu_texture_packer.svg)](http://badge.fury.io/rb/gosu_texture_packer)

[TexturePacker](http://www.codeandweb.com/texturepacker) support for [Gosu](https://github.com/jlnr/gosu) game engine.

## Installation

Add this line to your application's Gemfile:

    gem 'gosu_texture_packer'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install gosu_texture_packer

## Usage

```ruby
tileset = Gosu::TexturePacker::Tileset.load_json(gosu_window, '/path/to/tileset.json')
frame_names = tileset.frame_list
tile = tileset.frame(frame_names.first)
tile.draw(0, 0, 0) # tile is Gosu::Image
```

## Example Code

Run
[examples/tile_brush.rb](https://github.com/spajus/gosu-texture-packer/blob/master/examples/tile_brush.rb)
to see `gosu_texture_packer` in action.

Example tileset is loaded from
[spec/files](https://github.com/spajus/gosu-texture-packer/tree/master/spec/files) directory.

Click the window to draw random tiles.

![Gosu TexturePacker Example](https://raw.githubusercontent.com/spajus/gosu-texture-packer/master/examples/screenshots/tile_brush.png)

## Contributing

1. Fork it ( https://github.com/[my-github-username]/gosu_texture_packer/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
