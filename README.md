# Kasada's p.js Deobfuscated

The script was obfuscated by replacing most strings with a function to grab the string from an array and decode it.

Ex:
`_0x36f133(0x5ee,'m6n4')`

0x5ee is the index and "m6n4" is a value used to decode the string from the array.

The array is not in the correct order at first and it is rearranged when the script is first executed.

Note: Identifiers were replaced with more eye friendly ones
```js
;(function (juquana, jernae) {
    var gali = KPSDK_0x1a3a; // KPSDK_0x1a3a is the function that pulls from the array and decodes the string
    while (true) {
      try {
        var tuyetnhung = -parseInt(gali(1246, "ZrqT")) * parseInt(gali(1123, "SF8Y")) + parseInt(gali(866, "B&jL")) + parseInt(gali(488, "i&SL")) * parseInt(gali(749, "SF8Y")) + parseInt(gali(1404, "0mUP")) * parseInt(gali(1382, "VR1C")) + parseInt(gali(1566, "8%Ma")) * -parseInt(gali(937, "s$M0")) + parseInt(gali(1517, "KuSv")) * parseInt(gali(1258, "HY&U")) + -parseInt(gali(403, "s$M0")) * parseInt(gali(1201, "#jW1"));
        if (tuyetnhung === jernae) break; else juquana.push(juquana.shift());
      } catch (oshanna) {
        juquana.push(juquana.shift());
      }
    }
  }(KPSDK_0xf49f, 464424) // KPSDK_0xf49f is the array of encoded strings
```

The first element of the array gets sent to the back until the array is in the correct order or `tuyetnhung ==  464424`.

After deobfuscating:
```js
 ;(function (juquana, jernae) {
    while (true) {
      try {
        var tuyetnhung =
          -parseInt("2heZWMs") * parseInt("135654qTbABM") +
          parseInt("301063jmvAoT") +
          parseInt("11009YPscRF") * parseInt("81JRakrh") +
          parseInt("2Dxgobv") * parseInt("2215QuFPap") +
          parseInt("353049JvnAYK") * -parseInt("1tJFxcB") +
          parseInt("1201DTKmnY") * parseInt("547chHHWy") +
          -parseInt("18668hOnZuB") * parseInt("41zmWBxs");
        if (tuyetnhung === jernae) break;
        else juquana.push(juquana.shift());
      } catch (oshanna) {
        juquana.push(juquana.shift());
      }
    }
  })(KPSDK_0xf49f, 464424)
```

If you evaluate `tuyetnhung` yourself you will notice it equals `464424`.

Now that the array is in the correct order all of the following calls to `KPSDK_0x1a3a` can be replaced with their string value like shown above.

The next step of deobfuscating this script is coming up with a strategy to make the VM logic starting at line 1508 more readable.
#

Currently I'm not proud of the code I wrote for the deobfuscator so that will not be open sourced yet

To deobfuscate the script I used AST manipulation which you can learn more about [here](https://0x31.sh/)
#
Humphreyyyy#0088
