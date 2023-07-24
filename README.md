# mavbozo/clj-playaround-template

a template for my go-to deps.edn based development setup 

## Usage


This is a template project for use with [deps-new](https://github.com/seancorfield/deps-new).
As originally generated, it will produce a new library project `myusername/mycoollib` when run in your terminal:

    clojure -Sdeps '{:deps {com.github.mavbozo/clj-playaround-template {:git/sha "ab11efb4c39f4f7161db62dcaf0989d4d01b9319"}}}' -Tnew create :template mavbozo/clj-playaround-template :name myusername/mycoollib

Assuming you have installed `deps-new` as your `new` "tool" via:

```bash
clojure -Ttools install io.github.seancorfield/deps-new '{:git/tag "v0.5.2"}' :as new
```

> Note: once the template has been published (to a public git repo), the invocation will be the same, except the `:local/root` dependency will be replaced by a git or Maven-like coordinate.

Run this template project's tests (by default, this just validates your template's `template.edn`
file -- that it is valid EDN and it satisfies the `deps-new` Spec for template files):

    $ clojure -T:build test

## License

Copyright © 2023 Mavbozo

_EPLv1.0 is just the default for projects generated by `deps-new`: you are not_
_required to open source this project, nor are you required to use EPLv1.0!_
_Feel free to remove or change the `LICENSE` file and remove or update this_
_section of the `README.md` file!_

Distributed under the Eclipse Public License version 1.0.
