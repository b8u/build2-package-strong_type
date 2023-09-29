# strong_type
`build2` package for the [`strong_type`](https://github.com/rollbear/strong_type) C++ library.

## Usage

You can simply add this package as dependency to your project by specifying it in your `manifest`:

```
depends: string_type ^12.0.0
```

Then just pick the targets that you need:

```
import libs  = string_type%lib{string_type}
```

Make sure to add the stable section of the cppget.org repository to your project's repositories.manifest to be able to fetch the package.

```
:
role: prerequisite
location: https://pkg.cppget.org/1/stable
# trust: ...
```
