# poly-gradient

[![Buy Me a Coffee](http://static.tonybogdanov.com/github/coffee.svg)](http://ko-fi.co/1236KUKJNC96B)

[Demo & Documentation](http://tonybogdanov.github.io/poly-gradient/bower_components/poly-gradient/index.html)

`<poly-gradient>` provides a simple way of creating gradient backgrounds through a [Polymer](https://polymer-project.org) element.

Supports manually specifying color stops or presets loaded from an external JSON file.

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Playing With Your Element

If you wish to work on your element in isolation, it's recommended that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at `http://localhost:8080/components/poly-crypt/`.

## Example Usage

### Using `stops` attribute

    <poly-gradient angle="-90" stops='{"0":"#f00","1":"#0f0"}' width="320px" height="240px"></poly-gradient>
    
### Using `<poly-gradient-stop>` elements
    
    <poly-gradient angle="-75" width="320px" height="240px">
        <poly-gradient-stop offset="0" color="#f00"></poly-gradient-stop>
        <poly-gradient-stop offset="0.15" color="#ff0"></poly-gradient-stop>
        <poly-gradient-stop offset="0.3" color="#0f0"></poly-gradient-stop>
        <poly-gradient-stop offset="0.5" color="#0ff"></poly-gradient-stop>
        <poly-gradient-stop offset="0.65" color="#00f"></poly-gradient-stop>
        <poly-gradient-stop offset="0.8" color="#f0f"></poly-gradient-stop>
        <poly-gradient-stop offset="1" color="#f00"></poly-gradient-stop>
    </poly-gradient>
    
### Using a preset

    <poly-gradient preset="Sunset" width="320px" height="240px"></poly-gradient>