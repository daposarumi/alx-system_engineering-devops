# Shell init files, variables and expansions
## This set of command or scripts are pertaining to expansions, creating variables etc.

* `alias ls="rm*"` : script creates alias with name `ls` and `rm*` value<br>
* `echo hello $USER` : prints `hello user`. <br>
* `PATH=$PATH:/action` : adds `/action` to the path (last) <br>
* `echo $PATH | tr ":" "\n" | wc -l` : script counts number of diectories in path.<br>
* `env` : script lists environmenatal variables <br>
* `set`: script lists environmenatal variables, local variables and functions<br>
* `BEST="School"` : script creates local variable<br>
* `export BEST=School` : script creates global variable <br>
* `echo $((TRUEKNOWLEDGE + 128))` : prints result of 128 and environment variable `TRUEKNOWLEDGE`, followed by new line<br>
* `echo $((POWER/DIVIDE))` : script divides one envorionmental variable by another<br>
* `echo $((BREATH**LOVE))` : script prints the result of `BREATH` to the power of `LOVE`<br>
* `echo $((2#$BINARY))` : script converts number stored in environment varaible `BINARY` from base 2 to 10<br>
* `echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo` : script prints all possible combination of letters except `oo`, one combination per line <br>
* `printf "%0.2f\n" $NUM` : script prints number with two decimal places, followed by a new line. it will be stored in env. variable `NUM`<br>
* `printf '%x\n' $DECIMAL` : script converts a number from base 10 to base 16.<br>
* `tr 'A-Za-z' 'N-ZA-Mn-za-m'` : script encodes and decodes text using the rot13 encryption. Assume ASCII.<br>
* `paste -d" " - - | cut -d " " -f 1` : script every other line from the input, starting with the first line.<br>
* `printf "%o\n" $(( $((5#$(echo $WATER | tr water 01234))) + $((5#$(echo $STIR | tr stir. 01234))) )) | tr 01234567 bestchol \` : script adds the two numbers stored in the environment variables WATER and STIR and prints the result.
