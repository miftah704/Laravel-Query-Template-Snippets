# Laravel Query Template Snippets

improve your project.
* Laravel 9x.
* Laravel 8x.

## Example
-select()
```
    ->select('column1','column1')
```
-whereX()
```
    ->whereColumn('value...')
```

-with():multiple
```
    ->with(['table1:id','table2:id'])
```

-firstWhere()
```
    ->firstWhere('column', 'operator', 'value');
```

## Features

>**Collection Template Snippets**

| Collection                    |Collection                   |Collection           |
| ----------------------------  |----------------------------  |-------------------------- |
| `-all()`                      |`-keys()`                      |`-sortBy()`                |
| `-avg()`                      |`-last()`                      |`-sortDesc()`              |
| `-chunk()`                    |`-lazy()`                      |`-sortKeys()`              |
| `-collapse()`                 |`-map()`                       |`-splitIn()`               |
| `-collect()`                  |`-max()`                       |`-sum()`                   |
| `-combine()`                  |`-merge()`                     |`-take()`                  |
| `-concat()`                   |`-min()`                       |`-takeUntil()`             |
| `-contains()`                 |`-only()`                      |`-takeWhile()`             |
| `-count()`                    |`-pluck()`                     |`-tap()`                   |
| `-countBy()`                  |`-pop()`                       |`-times()`                 |
| `-crossJoin()`                |`-prepend()`                   |`-toArray()`               |
| `-diff()`                     |`-pull()`                      |`-toJson()`                |
| `-diffAssoc()`                |`-push()`                      |`-union()`                 |
| `-diffKeys()`                 |`-put()`                       |`-unique()`                |
| `-doesntContain()`            |`-replace()`                   |`-unwrap()`                |
| `-duplicates()`               |`-replaceRecursive()`          |`-value()`                 |
| `-every()`                    |`-reverse()`                   |`-values()`                |
| `-except()`                   |`-search()`                    |`-when()`                  |
| `-filter()`                   |`-shift()`                     |`-whenEmpty()`             |
| `-first()`                    |`-shuffle()`                   |`-whenNotEmpty()`          |
| `-firstOrFail()`              |`-skip()`                      |`-where()`                 |
| `-firstWhere()`               |`-skipUntil()`                 |`-where():operator         |
| `-flatMap()`                  |`-skipWhile()`                 |`-whereX()`                |
| `-flatten()`                  |`-slice()`                     |`-whereIn()`               |
| `-flip()`                     |`-sliding()`                   |`-whereBetween()`          |
| `-forget()`                   |`-sole()`                      |`-whereNotBetween()`       |
| `-forPage()`                  |`-sort()`                      |`-whereNotIn()`            |
| `-get()`                      |`-sortKeysUsing()`             |`-whereNotNull()`          |
| `-groupBy()`                  |`-splice()`                    |`-whereNull()`             |
|                               |`-wrap()`                      |`-orWhere()`               |
|                               |`-zip()`                       |`-orWhere():operator`      |


>**Query Template Snippets**

- xauth:user

```
    auth()->user()->id
```

-xcreate:template
```
    model::create([
        ''		=> value,
    ]);
```

xvalidation:template
```
    $validated = $request->validate([
	    ''		=> 'data',
    ]);
```

- xview:return

```
    return view('pages....', [
        ''		=> ,
    ]);
```

-xcreateMany:template
```
    $table->relation()->createMany([
        ''		=> value,
        ''		=> value
    ]);
```

- xredirect:route

```
    return redirect()->back()->with('messages',__('flash.insert'));
```

- xif:ternary
```
    ($condition) ? $statment1 : $statment2
```

- xgets:var
```
   $variable = 'query or data';
```

- xarray:3
```
    ''		=> ,
    ''		=> ,
    ''		=> ,
```


| query template               | query   template             | query template                 |
| ------------------------------| ------------------------------|  ------------------------------| 
| `xauth:user`                  |  `xarray:1`                    |  `xinsertGetId:template`       | 
| `xredirect:route`             |  `xarray:2`                    |  `xcreate:template`            | 
| `xredirect:back`              |  `xarray:3`                    |  `xupdate:template`            | 
| `xview:return`                |  `xgets:var`                   |  `xvalidation:template`        | 
| `xfunc:arrow`                 |  `xpublic:var`                 |   xcreateMany:template         | 
| `xarrtobj:template`           | `xif:ternary`                  |    xsave:template              | 
|                               | `xcreateInRelation:template`   | `xsaveMany:template`           |

#
>**Blade Template Snippets**

- xroute:multiple
```
    {{ route('route.name',[$variable1, $variable2, $variable3]) }}
```

- xlang:local
```
    {{ __('') }}
```

- xslot:anonymous
```
    <x-slot:>{{$variable}}</x-slot:>
```

- xslot:attribute
```
    <x-slot:heading class="">
	    heading
    </x-slot:heading>
```

- xlink:css
```
    <link href="{{ asset('style/...') }}" rel="stylesheet">
```

- xlink:js
```
    <script src="{{ asset('style/...') }}">
```

| blade template               | blade template               | blade template               |
| ---------------------------- | ---------------------------- | ---------------------------- |
| `xroute:single`              | `xslot:attribute`            | `xmodal:template`            |
| `xroute:multiple`            | `xlink:css`                  | `xcol:template`              |
| `xroute:non-attribute`       | `xlink:js`                   | `xrow:template`              |
| `xlang:local`                | `xbutton-toggle`             | `xcard:template`             |
| `xslot:anonymous`            | `xvariant:class`             | `xcontent:template`          |

## Authors

miftah shidiq

<!-- ## Acknowledgments -->