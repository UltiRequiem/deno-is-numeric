# is-number

[![CI](https://github.com/UltiRequiem/is-number/actions/workflows/ci.yaml/badge.svg)](https://github.com/UltiRequiem/is-number/actions/workflows/ci.yaml)
[![Code Coverage](https://codecov.io/gh/ultirequiem/is-number/branch/main/graph/badge.svg)](https://codecov.io/gh/ultirequiem/is-number)
[![Deno Doc](https://doc.deno.land/badge.svg)](https://doc.deno.land/https/deno.land/x/is_number/mod.ts)

[![Custom badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fdeno-visualizer.danopia.net%2Fshields%2Flatest-version%2Fx%2Fis_number%2Fmod.ts)](https://doc.deno.land/https/deno.land/x/is_number/mod.ts)

Check if an string is Numeric.

## Usage

### [Deno 🦕](https://deno.land/x/is_number)

```typescript
import { isNumber } from "https://deno.land/x/is_number/mod.ts";

isNumber("hello")); //=> false
isNumber("678")); //=> true
isNumber({}) //=> false
isNumber(+{a:"34"}) //=> false
isNumber(345)); //=> true
```

### [Node.js 🐢](https://npmjs.com/package/@ultirequiem/is-number)

```typescript
import { isNumber } from "@ultirequiem/is-number";
```

### Browser

Using
[type module](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)
🍱

- [esm.sh](https://esm.sh/@ultirequiem/is-number)

- [skypack](https://cdn.skypack.dev/@ultirequiem/is-number)

Using a plain
[script tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script) 👇

- [jsdelivr](https://cdn.jsdelivr.net/npm/@ultirequiem/is-number)

- [unpkg](https://unpkg.com/@ultirequiem/is-number)

You have the same API on all of this platforms.

## Documentation

[Autogenerated Documentation](https://doc.deno.land/https://deno.land/x/is_number/mod.ts)

### True Cases

```typescript
isNumber(5e3);
isNumber(0xff);
isNumber(-1.1);
isNumber(0);
isNumber(1);
isNumber(1.1);
isNumber(10);
isNumber(10.1);
isNumber(100);
isNumber("-1.1");
isNumber("0");
isNumber("012");
isNumber("0xff");
isNumber("1");
isNumber("1.1");
isNumber("10");
isNumber("10.10");
isNumber("100");
isNumber("5e3");
isNumber(parseInt("012"));
isNumber(parseFloat("012"));
```

### False cases

Everything else is false.

```typescript
isNumber(Infinity);
isNumber(NaN);
isNumber(null);
isNumber(undefined);
isNumber("");
isNumber("   ");
isNumber("foo");
isNumber([1]);
isNumber([]);
isNumber(function () {});
isNumber({});
```

See the [tests](./mod_test.ts) for more examples.

## Support

Open an Issue, I will check it a soon as possible 👀

If you want to hurry me up a bit
[send me a tweet](https://twitter.com/intent/tweet?text=%40UltiRequiem%20) 😆

Consider [supporting me on Patreon](https://patreon.com/UltiRequiem) if you like
my work 🚀

Don't forget to start the repo ⭐

## Licence

Licensed under the MIT License.
