# LibTal

Varvara/Uxn Uxntal Standard Library.

# Usage

Copy `libtal` in your project's root directory:

* **`root`**
  - _`libtal`_
  - `main.tal`

## Include **LibTal** header and footer.

```
~libtal/header


( variables )
|0000


( program )
|0100 ( -> ) [    
	;hello print-str

	HALT

	BREAK
] 


( data )
@hello "Hello \s "world! \n \0


~libtal/footer
```

### Minimal empty example.

```
~libtal/header


|0100


~libtal/footer
```

_Press `CTRL+C` to end this empty exmple rom, when run._

## Assemble and run.

```
$ uxnasm main.tal main.rom && uxncli main.rom
Assembled main.rom in 39 bytes(0.06% used), 115 labels, 30 macros.
Loaded main.rom
Hello world!
$
```
