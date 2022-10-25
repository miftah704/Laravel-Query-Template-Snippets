# Laravel Query Template

improve your project with laravel query template.

* Laravel 9x.
* Laravel 8x.

## Example
-select
```
    ->select('column1','column1')
```

-with:multiple
```
    ->with(['table1:id','table2:id'])
```

-firstWhere()
```
    ->firstWhere('column', 'operator', 'value');
```

-xcreate:template
```
    model::create([
        ''		=> value,
    ]);
```

-xcreateMany:template
```
    $table->relation()->createMany([
        ''		=> value,
        ''		=> value
    ]);
```
-xsaveMany:template
```
    $table->relation()->saveMany([
        new Model1(['column1' => 'value']),
        new Model2(['column1' => 'value'])
    ]);
```

xauth:user
```
    auth()->user()->id
```
xredirect:route
```
    return redirect()->route('')->with('messages',__('lang.success'));
```
xredirect:route
```
    return view('pages....', [
	    ''		=> ,
    ]);
```

xredirect:route
```
    model::create([
	    ''		=> data,
    ]);
```

xvalidation:template
```
    $validated = $request->validate([
	    ''		=> 'data',
    ]);
```


xroute:multiple
```
    {{ route('route.name',[$variable1, $variable2, $variable3]) }}
```

xlang:local
```
    {{ __('') }}
```

xslot:anonymous
```
    <x-slot:>{{$variable}}</x-slot:>
```

xslot:attribute
```
    <x-slot:heading class="">
	    heading
    </x-slot:heading>
```

## Features
Eloquent Template Snippets :
| Snippet                       |
| ----------------------------  |
| `-select()`                   |
| `-all()`                      |
| `-average()`                  |
| `-chunk()`                    |
| `-collapse()`                 |
| `-collect()`                  |
| `-combine()`                  |
| `-concat()`                   |
| `-contains()`                 |
| `-count()`                    |
| `-countBy()`                  |
| `-crossJoin()`                |
| `-diff()`                     |
| `-diffAssoc()`                |
| `-diffKeys()`                 |
| `-doesntContain()`            |
| `-duplicates()`               |
| `-every()`                    |
| `-except()`                   |
| `-filter()`                   |
| `-first()`                    |
| `-firstOrFail()`              |
| `-firstWhere()`               |
| `-flatMap()`                  |
| `-flatten()`                  |
| `-flip()`                     |
| `-forget()`                   |
| `-forPage()`                  |
| `-get()`                      |
| `-groupBy()`                  |
| `-with:single`                |
| `-with:multiple`              |
| `-withCount`                  |
| `-whereRelation`              |
| `-whereDoesntHave`            |

Query Template Snippets :
| Snippet                       |
| ------------------------------| 
| `xauth:user`                  | 
| `xredirect:route`             | 
| `xredirect:back`              | 
| `xview:return`                | 
| `xfunc:anonymous`             | 
| `xarray:1`                    | 
| `xarray:2`                    | 
| `xarray:3`                    | 
| `xgets:var`                   | 
| `xpublic:var`                 | 
| `xif:ternary`                 | 
| `xarrtobj:template`           | 
| `xinsertGetId:template`       | 
| `xinsertGetId:template`       | 
| `xcreate:template`            | 
| `xupdate:template`            | 
| `xvalidation:template`        | 


Blade Template Snippets | Custom:
| Snippet                      |
| ---------------------------- |
| `xroute:single`              |
| `xroute:multiple`            |
| `xroute:non-attribute`       |
| `xlang:local`                |
| `xslot:anonymous`            |
| `xslot:attribute`            |
| `xlink:css`                  |
| `xlink:js`                   |
| `xbutton-toggle`             |
| `xvariant:class`             |
| `xmodal:template`            |
| `xcol:template`              |
| `xrow:template`              |
| `xcard:template`             |
| `xcontent:template`        |

## Authors

miftah shidiq

<!-- ## Acknowledgments -->